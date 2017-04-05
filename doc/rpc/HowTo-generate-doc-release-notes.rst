================================================
How-To: Generate RPC documentation release notes
================================================

The purpose of the documentation release notes is to inform stakeholders about
changes in documentation between releases.

The process involves generating a changelog based on the RPC release tag.

$. Check merged pull requests are assigned the release tag that matches the
   RPC engineering release tag. For more information, see :ref:`tag-commits`.

$. Clone the docs-rpc repository:

   .. code::

      $ git clone https://github.com/rackerlabs/docs-rpc.git

   .. note::

      Clone the upstream docs-rpc repository. The changelog generator will not
      work correctly from a personal fork.

$. Create a new branch:

   .. code::

      $ git checkout -b NEWBRANCHNAME

$. In your local docs-rpc directory, install the GitHub Changelog Generator:

   .. code::

      $ gem install github_changelog_generator

$. `Generate a token <https://github.com/settings/tokens/new?description=GitHub%20Changelog%20Generator%20token>`_
    to allow more than 50 unauthenticated GitHub requests per hour.

$. Set the environment variable:

   .. code::

      $ export CHANGELOG_GITHUB_TOKEN="«your-40-digit-github-token»"

   .. note::

      For your convenience, set this variable in your :file:`bashrc` file.

$. Create a :file:`.github_changelog_generator` file to override the default
   parameters and configure your generated output. For example:

   .. code::

      header-label=# RPC Documentation Change Log
      unreleased=false
      issues=false
      author=false
      pr-label=### Documentation changes:

   For more information on parameters, see `Advanced change log generation
   examples <https://github.com/skywinder/github-changelog-generator/wiki/Advanced-change-log-generation-examples>`_

$. Run the changelog command to generate a :file:`changelog.md` file:

   .. code::

      $ github_changelog_generator

$. Edit the file to include only notable merged PRs. such as revisions
   and changes to technical information, migrated content, and changes to the
   content structure. Do not include editorial changes and changes to the
   documentation toolchain.

$. Convert the :file:`changelog.md` file to RST format using Pandoc:

   .. code::

      $ pandoc -s rst changelog.md -o changelog.rst

   .. note::

      Pandoc conversion is not perfect, so editing the file may be required to
      comply with RST conventions.

$. Add the :file:`changelog.rst` and :file:`.github_changelog_generator` files
   to your commit:

   .. code::

      $ git add changelog.rst .github_changelog_generator

$. Commit your changes:

   .. code::

      $ git commit

$. Push your commit to the docs-rpc repository:

   .. code::

      $ git push -u origin NEWBRANCHNAME

$. Go to the
   `GitHub docs-rpc repository <https://github.com/rackerlabs/docs-rpc.git>`_
   and create a pull request.
