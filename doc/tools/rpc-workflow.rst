============
RPC workflow
============

`docs-rpc <https://github.com/rackerlabs/docs-rpc>`_ is a private GitHub
repository that contains both external and internal-only content. The
repository has some extra configuration elements that enable us to
build both types of content from a single ``doc`` directory while also
providing access to multiple versions of the documentation.

As a result of this extra configuration, there are a few ways in which
docs-rpc interaction differs from our standard workflow.


Prerequisites
~~~~~~~~~~~~~

Tox is required for building, testing, and internal publishing:

.. code::

   $ sudo pip install tox


Using tox
~~~~~~~~~

`tox <https://tox.readthedocs.io/en/latest/>`_ is a Python tool for automated
testing. Although it is designed primarily for testing code, it is also useful
for testing and building docs.

Tox provides us with two main benefits:

-  it handles dependency installation, which enables us to avoid installing
   requirements locally and ensures we are all using the same package versions
-  it provides a virtual environment that can be reproduced on a variety of
   machines

In other words, if the documentation builds correctly in one tox environment,
it should build correctly in all tox environments.

Configuration
-------------

Tox configuration is controlled by a ``tox.ini`` file in the repository root.
It consists of general tox settings, a series of testenvs that can be
invoked individually (e.g. ``tox -e checkbuild``), and configuration for
certain tests.

For our purposes, this file is relatively simple:

.. code::

   [tox]
   minversion = 1.6
   envlist = checksyntax,checkbuild
   skipsdist = True

   [testenv]
   deps = -r{toxinidir}/requirements.txt

   whitelist_externals =
     bash
     make

   [testenv:checkbuild]
   commands =
     make html -C {toxinidir}/doc

   [testenv:checklinks]
   commands =
     make linkcheck -C {toxinidir}/doc

   [testenv:checkspelling]
   commands =
     make spelling -C {toxinidir}/doc

   [testenv:checksyntax]
   commands =
     doc8 doc

   [testenv:checkversions]
   commands =
     sphinx-versioning build {toxinidir}/doc {toxinidir}/doc/_build/html

   [testenv:publish]
   commands =
     sphinx-versioning push {toxinidir}/doc gh-pages .

   [doc8]
   # Ignore target directories
   ignore-path = doc/_build*
   # File extensions to use
   extensions = .rst,.txt
   # Maximal line length is 79.
   max-line-length = 79
   # Disable D000: Check RST validity (cannot handle lineos directive)
   # ignore = D000

Description of tox.ini options
------------------------------

[tox]
   - **minversion**: minimum version of tox to use
   - **envlist**: testenvs to run when none are specified. I.e. when you run
     ``tox``.
   - **skipdist**: run tox without requiring a ``setup.py`` file

[testenv]
   - **deps**: packages required by all testenvs. We install them from the
     ``requirements.txt`` file.
   - **whitelist_exernals**: commands sourced from the local operating system
     instead of being downloaded and installed by tox

[testenv:NAME]
   - **checkbuild**: build the current branch using ``make html``.
     Configuration is in ``conf.py`` and ``Makefile``.
   - **checklinks**: run link checker. Configuration is in ``conf.py``.
   - **checkspelling**: run spell checker. Configuration is in ``Makefile`` and
     the custom dictionary is ``spelling_wordlist.txt``
   - **checksyntax**: run RST syntax check. Configuration is in ``tox.ini``.
   - **checkversions**: build versioned docs. Configuration is in ``conf.py``.
   - **publish**: builds the documentation and pushes it to the our internal
     gh-pages site. Configuration is in ``conf.py``. Using this command has
     special requirements. See `Publishing`_.

[doc8]
   - configuration options for the doc8 tests run in the checksyntax env

Troubleshooting
---------------

In order to run more quickly, tox reuses elements of its virtual test
environment. This makes sense, as there is no need to re-download all the
packages required for building the docs if the requirements have not changed.
However, when a configuration option changes or a new package is available,
tox does not automatically refresh its environment.

If you or someone else changes a configuration option in ``tox.ini`` or alters
the ``requirements.txt`` file, you must force tox to recreate the test
environment. You can do this in two ways:

-  Add the ``-r, --recreate`` option the next time you run tox:

   .. code::

      $ tox -r

-  Delete the hidden ``.tox`` directory in the repository root where the
   environment is stored:

   .. code::

      $ rm -rf .tox

Most of the time, recreating the tox environment solves tox-related problems.
If you are still having issues, check the configuration in ``tox.ini``
is correct.

On rare occasions, a new version of an upstream dependency causes a failure
when installing from ``requirements.txt``. The tox error output should provide
some clue in the traceback. Package maintainers will usually fix it these sorts
of errors fairly quickly. In the meantime, you can pin that package to the
most recent working version in ``requirements.txt``. For example:

.. code::

   sphinx<=1.4.1
   sphinx_rtd_theme==0.1.9

If you do this, please retest every few days and remove the version requirement
when the package is fixed.


Local builds
~~~~~~~~~~~~

You have three options for building the current working branch.

The recommended approach is using ``tox``, which loads all requirements into
a virtual environment. Tox commands can be run from any location within the
docs-rpc repository.

-  Run syntax checks and build the docs (recommended):

   .. code::

      $ tox

-  Build the docs without syntax checks (slightly faster):

   .. code::

      $ tox -e checkbuild

Tox builds the documentation by calling ``make html``. You can, however, run
the make command directly if required. Before doing this, you need to install
locally all the dependencies listed in the ``requirements.txt`` file. This only
needs to be done once, but you should regularly update your installed packages
to the latest versions while keeping them in sync with any pinned dependencies
in ``requirements.txt``:

.. code::

   $ sudo pip install -r requirements.txt

You can then build the documentation by changing into the ``doc`` directory and
running ``make``:

.. code::

   $ make html

View the built documentation by opening ``doc/_build/html/index.html``
in your browser.


Advanced local builds
~~~~~~~~~~~~~~~~~~~~~

The basic `local builds`_ options are sufficient for testing changes on your
current working branch before creating a pull request.

However, the basic build *only* builds the current working branch, and we
have several versions of the RPC docs on stable branches. When we publish to
the internal gh-pages site, we publish all the stable branches using a single
index page with a version selector.

You can build the versioned site locally, but there are a few extra steps you
must take:

#. Add your working branch to the whitelist.
#. Push your branch to origin before building.
#. Build the versioned documentation site.
#. Remove your working branch from the whitelist before creating a PR.


Adding your working branch to the whitelist
-------------------------------------------

Versioned builds are created using `SCVersioning
<https://robpol86.github.io/sphinxcontrib-versioning>`_, which is configured
in ``conf.py``:

.. code::

   scv_root_ref = 'v13'
   scv_overflow = ('-q', )
   scv_show_banner = True
   scv_banner_main_ref = 'v13'
   scv_whitelist_branches = (re.compile(r"\bmaster\b|\bv1[123]\b"),)
   scv_whitelist_tags = ('NIL', )
   scv_push_remote = 'internal'
   scv_grm_exclude = ('.nojekyll', '.gitignore')

Our interest here is ``scv_whitelist_branches``. For information about the
other configuration options, see `sphinxcontrib-versioning options
<https://robpol86.github.io/sphinxcontrib-versioning/settings.html>`_.

SCVersioning works by reading the list of whitelisted branches and building
each one as a version of the documentation suite. If you are on a working
branch, you must add it to the whitelist in order to include it in the build.

Adding ``v12`` to the whitelist matches all branches with ``v12`` in them. For
example, ``testv12`` and ``v12-wip``. To prevent such matches, we use a regular
expression that matches only branches with the exact names given. Currently the
expression matches ``master``, ``v11``, ``v12``, and ``v13``.

While testing your content, you may also want to remove some of the other
branches to speed up local builds. Commenting out the production list makes
it easier to restore later.

Assuming a working branch named ``issue-123``, you could use:

.. code::

   # scv_whitelist_branches = (re.compile(r"\bmaster\b|\bv1[123]\b"),)
   scv_whitelist_branches = (v13, issue-123)

While you can remove most branches during testing, you must keep the branch
designated as ``scv_root_ref``, as this is the branch treated as the default
version. Normally, this is the latest release of the RPC docs.

Pushing to origin
-----------------

SCVersioning only works with remote branches and ignores local changes
(committed, staged, unstaged, etc). You must push your work to origin or
SCVersioning cannot see it. This eliminates race conditions when multiple CI
jobs are building docs at the same time.

After you commit you work locally, push it to origin:

.. code::

   $ git push --set-upstream origin issue-123

You only need to set the upstream once. For pushing subsequent commits
to origin, use:

.. code::

   $ git push

Building the versioned site
---------------------------

SCVersioning uses its own build command to produce the versioned site. The
recommended way to invoke it is using the ``checkversions`` tox environment:

.. code::

   $ tox -e checkversions

Alternatively, you can run the build command directly from the repository root,
but the same caveats apply regarding dependencies as running ``make html``
directly:

.. code::

   $ sphinx-versioning build doc doc/_build/html

Open ``doc/_build/html/index.html`` in a browser to view the versioned site.
Use the version selector to view your branch and see the latest changes.

.. important::

   Before building the versioned site, you must update the stable branches
   (e.g. ``v11``, ``v12``, ``v13``) locally then push them to origin in order
   to see the latest changes.

Removing your working branch from the whitelist
-----------------------------------------------

When you are finished testing and you are ready to create a pull request, you
must remove your branch from the whitelist and restore the list of stable
branches. Commit, push, then open your PR.

.. code::

   scv_whitelist_branches = (re.compile(r"\bmaster\b|\bv1[123]\b"),)

Reviewers can check your content using the Nexus preview. If they need to see
the internal gh-page styling or the versioned build, they must clone your fork
and build using the above workflow.


Publishing
~~~~~~~~~~

Publishing externally to `developer.rackspace.com
<https://developer.rackspace.com/docs/>`_ happens automatically when a PR is
merged into docs-rpc.

Publishing internally to `github.rackspace.com
<https://pages.github.rackspace.com/rpc-internal/docs-rpc/>`_ requires a few
extra steps.

Initial repository setup for internal publishing
------------------------------------------------

Publishing to the internal gh-pages site uses two remote repositories:

`rackerlabs/docs-rpc <https://github.com/rackerlabs/docs-rpc>`_
   a private repository on *github.com* where RPC documentation is developed

`rpc-internal/docs-rpc <https://github.rackspace.com/rpc-internal/docs-rpc>`_
   an internal repository on *github.rackspace.com* that is only accessible to
   users on the Rackspace network. This repository hosts our `internal gh-pages
   site <https://pages.github.rackspace.com/rpc-internal/docs-rpc/>`_.

.. warning::

   Do not edit the internal repository directly.

Run the following commands while connected to the Rackspace network directly
or through VPN. You only need to perform these steps once.

#. Upload an SSH key to your internal GitHub account. You can access SSH key
   options by going to **Settings -> SSH keys** in the GitHub interface.

#. Ask an RPC writer to add you to the **rpcdocs** team. This membership gives
   you push access to the **rpc-internal** repository.

#. In your local **docs-rpc** repository, add the internal repository as a
   remote:

   .. code::

      $ git remote add internal git@github.rackspace.com:rpc-internal/docs-rpc.git

#. Confirm your remote setup:

   .. code::

      $ git remote -v
      internal	git@github.rackspace.com:rpc-internal/docs-rpc.git (fetch)
      internal	git@github.rackspace.com:rpc-internal/docs-rpc.git (push)
      origin	git@github.com:username/docs-rpc.git (fetch)
      origin	git@github.com:username/docs-rpc.git (push)
      upstream	git@github.com:rackerlabs/docs-rpc.git (fetch)
      upstream	git@github.com:rackerlabs/docs-rpc.git (push)

#. Update your remotes:

   .. code::

      $ git remote update

#. Create a local **gh-pages** branch that tracks **internal/gh-pages**:

   .. code::

      $ git branch gh-pages --track internal/gh-pages

You are now ready to publish the RPC docs internally.

Publishing internally
---------------------

#. Update the stable branches (e.g. ``v12``, ``v13``, ``v14``). You
   can use the following script:

   .. code-block:: bash

      #!/bin/bash

      # Merges upstream into local stable branches and pushes the
      # results to origin.
      #
      # NOTE: the local branches (v12, v13, ...) must exist before
      # running this script


      branches=(v12 v13 v14)
      echo

      for item in ${branches[@]}; do
          git checkout $item
          git fetch upstream
          git merge upstream/$item
          git push origin $item
      done

      git checkout master
      git branch
      echo

#. Run the publish command from the master branch while connected to
   the Rackspace network directly or through VPN:

   .. code::

      $ tox -e publish


Using conditionals
~~~~~~~~~~~~~~~~~~

In order to have both internal and external documents in a single directory,
we use the `ifconfig <http://www.sphinx-doc.org/en/1.4.8/ext/ifconfig.html>`_
directive to label content that should only be published internally.

Configuration
-------------

Sphinx includes content labeled ``internal`` based on configuration settings
in ``conf.py``:

.. code::

   # set ifconfig tags
   if not 'CONTENT_ID_BASE' in os.environ or 'build-' in os.environ['CONTENT_ID_BASE']:
       # Nexus previews, gh-pages, and local builds
       internal = True
   else:
       # Nexus publishing
       internal = False

   ...

   def setup(app):
       """Create the internal config value and set to False."""
       app.add_config_value('internal', False, 'env')

Usage
-----

Use ``ifconfig`` like other directives, indenting content beneath it that you
want to apply to internal documents only.

For example:

.. code::

   This is some text that will appear in internal and external documentation.

   .. ifconfig:: internal

      This text will only appear in internal documenation.

Currently, we have completely separate books for internal and external
content. We only use this directive to conditionalize the ``doc/index.rst``
file.

Excluding internal documents from public builds
-----------------------------------------------

Although documents labeled with ``ifconfig`` in a toctree do not appear in
the external table of contents, the source is still processed and
output to the build directory. This means that the internal content can be
accessed externally through searches.

To prevent this, directories containing internal books must be excluded from
external builds by adding them to a conditional ``exclude_patterns`` list in
``conf.py``:

.. code::

   if internal is False:
       exclude_patterns.extend(['rpc-faq-internal', 'rpc-install-internal',
                               'rpc-ops-internal', 'rpc-sales-eng-internal',
                               'rpc-upgrade-exp'])

Due to these files being excluded, when Strider runs a merge build it will
output some ``nonexisting document`` and ``undefined label`` warnings. You
can safely ignore these.

.. code::

   ./index.rst:36: WARNING: toctree contains reference to nonexisting document 'rpc-faq-internal/index'
   ...
   ./index.rst:31: WARNING: undefined label: rpc-faq-internal (if the link has no caption the label must precede a section header)


Deconst global table of contents
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Deconst builds two tables of contents for Sphinx projects:

-  the main text area uses the table of contents provided by ``doc/index.rst``.
   A ``.. toctree::`` directive with the ``:hidden:`` option does not appear.
-  the sidebar uses a global table of contents. Normally this is built from
   ``doc/index.rst``. However, the global table of contents does not honor the
   ``:hidden:`` option, thus hidden toctrees appear in the sidebar. To avoid
   this, a special ``_toc.rst`` file is used to specify the sidebar table of
   contents. For more information, see
   https://deconst.horse/writing-docs/author/sphinx/#tables-of-contents.
