.. _tag-commits:

==============================
How-To: Tag RPC GitHub commits
==============================

Release tags are assigned to `docs-rpc <https://github.com/rackerlabs/docs-rpc>`_
commits to produce RPC documentation release notes using the
GitHub Changelog Generator <https://skywinder.github.io/github-changelog-generator/>`_
tool.

Release tags are defined as a major release (vN.n.n), minor release
(vn.N.n), revision release (vn.n.N), or release candidate (v.n.n.nrcN).

.. note::

   Please check the release tags in docs-rpc match RPC engineering release
   tags. For example, see https://github.com/rcbops/rpc-openstack/tags.

Creating a release tag on your current branch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Using the command line (assuming you are working from a personal fork):

#. On your current branch, create the release tag. For example:

   .. code-block:: console

      $ git tag -a r14.0

#. Push the tag to your personal fork and docs-rpc:

   .. code-block:: console

      $ git push origin --tags
      $ git push upstream --tags

#. Commit your branch changes.

Creating a release tag in GitHub
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the GitHub web interface:

#. Go to https://github.com/rackerlabs/docs-rpc/releases and click on
   :guilabel:`Draft a new release`.
#. Complete the form fields and click :guilabel:`Publish release`.

Tagging commits
~~~~~~~~~~~~~~~

In a series of merged commits to a branch, the last commit is tagged
for the latest release. For example:

...
commit6
commit5 <-- tagged as r14.0.0
commit4
commit3
commit2 <-- tagged as r14.0.0rc1
commit1
...

At the end of the sprint milestone or development release cycle, tag commits
in each branch with a release tag.

In the command line:

#. Update your local branch:

   .. code-block:: console

      $ git checkout BRANCH
      $ git fetch upstream
      $ git merge upstream/BRANCH

#. List the commit history. For example:

   .. code-block:: console

      $ git log --pretty=oneline

      0d10239da4eb58f3a3f261bd9fa8264e9599c0d2 Add note about nova_cross_az_attach (#1011)
      11157ed42c10e20b3e072e8620e457528224214e Include remote RPC README file (#1008)
      fd9066df2b6ee2ba86a2e3d9693efe3aa2b175d0 Add rc2 changelog (#1006)
      3fd3468579c6280391b6921e85ef7f19403079ed Update external LB link because page moved (#1007)
      439953ff4f4394c2c97b91a627353b57d58aa38d Update pre-req with env.d directory creation (#1005)
      5b78a9a2f91c63b2133805f3c833815051cf1105 Fixes title for Magnum API monitoring (#1000)
      65a12930720c4a7678d6fb1d8f44e96bb8c822d6 Remove external Ops Guide from master (#993)
      822d369ba29744173933c7415ac2c3d709bda76d Config updates (#1001)
      090f0625f8f0fddeb40b19a70fa41caf0b1e7233 Remove and redirect to standalone monitoring design docs (#999)
      a298933fde9a33c1d7fc8a76878c0ca9a24eea56 Draft Monitoring and Logging Guide (#914)
      e793f65d409c69d8f4f18cfff974654ab646aa5c Add known issues note about holland backup (#994)
      e36356d6b37d300dc080b62a649c1cf05a6e09c6 Adds release note for swift workaround (#991)
      144ac0cd43dea62e6e6581f26bbfd742bacb5c06 Fix backward ending slash; indentation (#990)

#. Search commits with a release tag. For example:

   .. code-block:: console

      $ git show r14.0

      commit 0d10239da4eb58f3a3f261bd9fa8264e9599c0d2
      Author: Alex Cantu <miguel.cantu@rackspace.com>
      Date:   Thu Mar 30 15:09:10 2017 -0500

         Add note about nova_cross_az_attach (#1011)

         Connects https://github.com/rcbops/rpc-openstack/issues/2095

#. For untagged commits, add the release tag referencing part of the
   commit checksum. For example, if commit #993 applies to r14.0:

   .. code-block:: console

      git tag -a r14.0 65a1293

#. Push tagged commits to docs-rpc and your personal fork:

   .. code-block:: console

      $ git push --tags upstream BRANCH
      $ git push --tags origin BRANCH
