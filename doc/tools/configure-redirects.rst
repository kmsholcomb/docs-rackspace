.. _configure-redirects:

===================
Configure redirects
===================

Deconst control repositories specify the configuration for each site managed
by a deconst instance. When you move or delete content from a site, add a
redirect rule to the `rewrites JSON files`_ for the site that hosts the
content so that users requesting access to the deleted content are
sent to a new location instead of getting a 404.

The rewrites files manage redirects for traffic to the following domains:

Active sites:

- support.rackspace.com
- developer.rackspace.com,
- getcarina.com.

Archived sites:

- docs.rackspace.com
- api.rackspace.com

Each file contains the rewrite rules for the specified domain, for example
``developer.rackspace.com.json`` specifies the rules to rewrite URLs or
URL patterns from that site to a specified URL.

For each rule, the ``from`` parameter specifies the URL to
be redirected. The ``to`` parameter specifies the target destination for the
redirected link.

**Example: Redirect traffic from a legacy Cloud Images API developer guide link**

.. code-block:: javascript

   {
      "description": "Redirect images developer-guide URL",
      "from": "^\\/docs\\/cloud-images\\/v2\\/developer-guide\\/(.*?)",
      "to": "/docs/cloud-images/v2/$1",
      "rewrite": false,
      "status": 301
   },

This example from the developer.rackspace.com redirects file, redirects any
URL that matches the following pattern:

``https://developer.rackspace.com/docs/cloud-images/v2/developer-guide/*.*``

to the following URL:

``https://developer.rackspace.com/docs/cloud-images/v2/<filename>``

This rule specifies the ``$1`` pattern to append the final node
of the original URL to the new path.

For example, a request for the following URL:

``https://developer.rackspace.com/docs/cloud-images/v2/developer-guide/glossary/``

redirects the user to the following URL:

``https://developer.rackspace.com/docs/cloud-images/v2/glossary/``


.. note::

   You can specify redirect rules by using glob patterns to match a set of
   URLs that you want to redirect. For information about understanding and
   using glob patterns, see `globby npm module`_ and `wildcard reference`_.

.. _Wildcard reference: http://www.tldp.org/LDP/GNU-Linux-Tools-Summary/html/x11655.htm
.. _globby npm module: https://www.npmjs.com/package/globby

Configure a redirect rule
~~~~~~~~~~~~~~~~~~~~~~~~~~~

When you add a redirect rule, place the rule in the order that you want it
processed. For example, if you have a specific redirect rule for a deep link,
you want to process that rule before a more general rule.

For example, if you have a set of rules to redirect traffic from the same
documentation project, place a rule to redirect a specific page in the content
above a rule that redirects the top-level page as shown in the following
example.

**Example: Order redirect rules**

.. code:: JSON

   {
      "description": "Reach Cloud Monitoring Metrics API Link",
      "from": "^/cm/api/v1.0/cm-devguide/content/metrics-api.html",
      "to": "/docs/rackspace-monitoring/v1/api-reference/metrics-operations/",
      "toProtocol": "https",
      "toHostname": "developer.rackspace.com",
      "rewrite": false,
      "status": 301
   },
   {
      "description": "Cloud Monitoring Developer Guide",
      "from": "^/cm",
      "to": "/docs/rackspace-monitoring/v1/",
      "toProtocol": "https",
      "toHostname": "developer.rackspace.com",
      "rewrite": false,
      "status": 301
      },

In this example, the first rule redirects a link from the Monitoring Metrics
API topic on the legacy docs.rackspace.com site to the new location on
developer.rackspace.com.

The second rule directs all links to the legacy Monitoring documentation to
the Monitoring documentation index page on developer.rackspace.com.

If these rules were reversed, the second rule would never be processed
because all traffic to the legacy Monitoring Guide would be redirected to
the index page and the more specific rule would not be processed.

Add a redirect rule
-------------------

Complete the following steps to add a rewrite rule:

#. Fork and clone the nexus-control repository.

#. On your local system, navigate to the following directory:
   ``config/rewrites.d``.

#. Edit the rewrites file for the site that controls the traffic you want to
   redirect.

#. Determine where to add the rule.

   - Find similar rules and insert or append your rule to that group.
   - Verify that traffic from the specified location won't be redirected
     by a preceding rule.

#. Add the rule.

   If you are redirecting a URL from one domain to another, make sure
   that you specify the ``ToHostName`` parameter in the redirect rule.

#. Commit your changes and push to GitHub.

#. Submit a pull request to the nexus-control repository.

#. After your updates are approved and merged, verify that the
   updates have been applied.


Test a redirect rule
~~~~~~~~~~~~~~~~~~~~

When you merge an update to the nexus-control configuration, it
can take time for the changes to be deployed to production.
You can check the status of the update in `nexus-control build results`_.
When the updates have been successfully deployed, the log shows the
following message:

.. code:: console

   Done, without errors.
   Asset preparer completed. { status: 0 }
   All assets from repository uploaded.

After the changes are deployed to production, test the redirect rule.

In the browser, navigate to a URL that matches the one specified in the
``from`` parameter of the redirect rule and verify that the browser directs you
to a URL that matches the one specified in the ``to`` parameter.

If the browser returns a 404 page or a different URL, update the rewrite file
to fix the issue.

.. _nexus-control build results: https://build.developer.rackspace.com/rackerlabs/nexus-control/

Troubleshoot rewrites file
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**After updating a rewrite file, all legacy links return 404**

If you have a missing comma or other syntax error in the rewrite JSON file,
the redirect configuration does not work.

To resolve the problem, use a `JSON linter`_ to verify the rewrite file syntax.

If you don't find any errors, make sure that you have a comma between redirect
rules as shown in the following example from the api.rackspace.com rewrites
file.

.. code-block:: javascript

   {
      "api.rackspace.com": [
            {
               "description": "Redirect root traffic to developer.rs.com/docs/",
               "from": "^\\/$",
               "to": "/docs/",
               "rewrite": false,
               "status": 301
            },
            {
               "description": "Cloud Servers redirect",
               "from": "^\\/(api-ref(\\.html)?)?$",
               "to": "/docs/cloud-servers/v2/developer-guide/",
               "rewrite": false,
               "status": 301
            },
            {
               "description": "Cloud Servers extensions redirect",
               "from": "^\\/api-ref-servers-ext(\\.html)?$",
               "to": "/docs/cloud-servers/v2/developer-guide/",
               "rewrite": false,
               "status": 301
            }
         ]
   }

.. note::

   You do not need a comma after the last rule. Also, delete any blank
   lines at the end of the file.

**Individual rule redirect incorrectly or returns 404**

Review the rewrites file to verify that the configuration for the redirect rule
is valid. Check the glob patterns and file syntax and fix any errors that
affect the rewrite rule processing service.



.. _rewrites JSON files: https://github.com/rackerlabs/nexus-control/tree/master/config/rewrites.d
.. _JSON linter: http://jsonlint.com/
