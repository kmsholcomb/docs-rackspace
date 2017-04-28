==================
Reno release notes
==================

Reno organizes notes into logical groups based on whether they describe
new features, bug fixes, known issues, or other topics of interest
to the user. Contributors categorize individual notes as they are
added, and reno combines them before publishing.

The RPC developer team writes release notes concurrently with development
patches. Notes are styled using reStructuredText directives, and reno’s
Sphinx integration makes it easy to incorporate release notes into
automated documentation builds.

For more details, see the official
`reno documentation <https://docs.openstack.org/developer/reno/>`_.

Installation
~~~~~~~~~~~~

At the command line:

.. code-block:: console

   $ pip install reno

To use the Sphinx extension built into reno, install the [sphinx] extra
dependencies:

.. code-block:: console

   $ pip install 'reno[sphinx]'

Usage
~~~~~

The reno command line tool is used to create a new release note file in
the correct format and with a unique name. The new subcommand combines
a random suffix with a “slug” value to create the file with a unique
name that is easy to identify again later.

.. code-block:: console

    $ reno new SLUG

    Created new notes file in releasenotes/notes/slug-goes-here-95915aaedd3c48d8.yaml

The ``--edit`` option opens the new note in a text editor:

.. code-block:: console

   $ reno new slug-goes-here --edit

   ... Opens the editor set in the EDITOR environment variable, editing the new file ...

   Created new notes file in releasenotes/notes/slug-goes-here-95915aaedd3c48d8.yaml

By default, the new note is created under ``./releasenotes/notes``. 
The ``--rel-notes-dir`` command-line flag changes the parent directory
(the notes subdirectory is always appended). It’s also possible to set a
custom template to create notes.

For more configuration options, see
`configuring reno <https://docs.openstack.org/developer/reno/usage.html#configuring-reno>`_.

Generating a report
~~~~~~~~~~~~~~~~~~~

To run a reno report to generate a report containing the release notes,
execute the following:

.. code-block:: console

   $ reno report <path-to-git-repository>

.. note::

   The ``--branch`` argument can be used to generate a report for a specific
   branch (the default is the branch that is checked out). To limit the report
   to a subset of the available versions on the branch, use the ``--version``
   option (it can be repeated).


