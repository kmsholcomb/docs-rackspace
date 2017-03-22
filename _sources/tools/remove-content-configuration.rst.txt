=====================================================
Remove a Sphinx documentation project from production
=====================================================

To delete published content from the nexus, make the following
configuration changes to the landing page, nexus-control repository, and
the content store:

#. Update the landing page index to delete the title from the html source.

   If you are removing a category, remove any associated sections or headings.
   For details, see the `landing page contribution guidelines`_.

#. To prevent 404 errors from existing links and bookmarks, update
   the ``rewrites.json`` file to add a
   :ref:`redirect rule <configure-redirects>`.

   - If the content has been moved to an external site, redirect the old
     URL to the URL on the new site.

   - If the content is no longer available, redirect the old URL to a logical
     reference point like the home page for the documentation collection.
     If necessary, you can add a page or topic to explain the content removal
     so that you can redirect links from the legacy content to the
     explanation.

#. :ref:`Delete content <delete-nexus-content>` that has already been deployed
   to ``developer.rackspace.com``.


Housekeeping tasks
~~~~~~~~~~~~~~~~~~~

Update the nexus control configuration to remove references to obsolete
projects.

#. Remove any project-specific entries from the nexus-control
   `content mapping`_ (``content.d``) and `template`_ (``route.d``) JSON files.

   You don't have to update these files if your project is configured in a
   group unless you want to remove the whole group. For example, to
   stop publishing all Rackspace Private Cloud v11 projects, delete
   the content mapping for the v11 branch of the docs-rpc GitHub repository.
   If you want to stop mapping private cloud content, remove the
   ``docs/private-cloud`` entry from the template file.

#. If you are removing an entire repository or branch within a repository,
   edit the Strider build job inventory in the ``content-repositories.json``
   file to remove the GitHub repository or branch name.


.. _landing page contribution guidelines: https://github.com/rackerlabs/docs-quickstart/blob/master/CONTRIBUTING.md
.. _content mapping: https://github.com/rackerlabs/nexus-control/blob/master/config/content.d/developer.rackspace.com.json
.. _template: https://github.com/rackerlabs/nexus-control/blob/master/config/route.d/developer.rackspace.com.json
.. _Strider build job inventory: https://github.com/rackerlabs/nexus-control/blob/master/content-repositories.json
.. _nexus-control configuration files: https://github.com/rackerlabs/nexus-control/tree/master/config


.. _delete-nexus-content:

Delete content from nexus content store
---------------------------------------

Use these instructions to delete content that has been deployed to a production
site managed by the nexus control repository.


Prerequisites
^^^^^^^^^^^^^

* You need an API key for the content service.
* You can't be on the VPN (because it blocks port 9000).
* It's helpful to have some kind of JSON formatter for your browser like
  the `Chrome JSON formatter`_.
* A `URL encoder`_ of some kind. I personally use the
  `escape-utils Atom package`_.

.. _Chrome JSON formatter: https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa
.. _URL encoder: http://meyerweb.com/eric/tools/dencoder/
.. _escape-utils Atom package: https://atom.io/packages/escape-utils

.. _list-content:

List content
^^^^^^^^^^^^

Before deleting content in production, it's a good idea to make sure you know
what you're about to delete. You can list the content IDs that are currently
present in Nexus by visiting the `content endpoint`_.

List content IDs that begin with a specific base by providing a URL-encoded
``?prefix=`` parameter as shown in the following example:

.. code:: console

    https://developer.rackspace.com:9000/content?prefix=https%3A%2F%2Fgithub.com%2Frackerlabs%2Fdocs-dedicated-vcloud>`_

Results are returned 100 at a time. You can paginate (awkwardly) by adding
``&pageNumber=2`` to the end of the URL. The full documentation is in
`content service README`_.


.. _content endpoint: https://developer.rackspace.com:9000/content/](https://developer.rackspace.com:9000/content/>
.. _content service README: https://github.com/deconst/content-service#get-contentprefixid_prefixpagenumbernumperpagesize


.. _delete-content:

Delete content
^^^^^^^^^^^^^^

Delete individual envelopes by submitting a cURL ``DELETE`` request to the
content service API, using the URL-encoded content ID:

.. code:: console

   export APIKEY="..."

   curl -X DELETE \
        -H "Authorization: deconst ${APIKEY}" \
        https://developer.rackspace.com:9000/content/https%3A%2F%2Fgithub.com%2Frackerlabs%2Fdocs-dedicated-vcloud

(You can copy and paste the ``/content/...`` bit from the ``url`` key in the
search results in your browser.)

To bulk delete *all* envelopes beneath a content ID base that you've removed or
renamed, specify the ``?prefix=true`` parameter:

.. code:: console

   export APIKEY="..."

   curl -X DELETE \
        -H "Authorization: deconst ${APIKEY}" \
        https://developer.rackspace.com:9000/content/https%3A%2F%2Fgithub.com%2Frackerlabs%2Fdocs-dedicated-vcloud?prefix=true

The documentation for this endpoint is also in
`the content service README <https://github.com/deconst/content-service#delete-contentidprefixtrue>`_.
