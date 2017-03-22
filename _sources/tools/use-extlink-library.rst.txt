.. _prepare-dev-guides-for-nexus:

=============================
Linking to external resources
=============================

We are using the `Sphinx external link library extension`_ to create a library
of common URL references that can be used to create link references to external
resources.

Using the link library provides these advantages:

- If the URLs to common resources change, you can update the external link
  library URL specification in the configuration file instead of having to
  update every link to that resource in the documentation library.

- Link references are shorter so you don't have to make as many format
  adjustments in tables and indented list to accommodate wrapping link text.

The link library URL specification is defined in the Sphinx configuration file
for each project.

**Example: Common external link library definition from the Sphinx
configuration file**

.. code-block:: python

   # External link library

   extlinks = {
      'rax': ('https://www.rackspace.com/%s', ''),
      'rax-cart': ('http://cart.rackspace.com/%s', ''),
      'rax-special': ('https://%s.rackspace.com/', ''),
      'rax-cloud': ('https://www.rackspace.com/cloud/%s', ''),
      'rax-dev': ('https://developer.rackspace.com/%s', ''),
      'rax-devdocs': ('https://developer.rackspace.com/docs/%s', ''),
      'rax-api':
        ('https:/developer.rackspace.com/docs/%s/api-reference', ''),
      'rax-git': ('https://github.com/rackspace/%s', ''),
      'mycloud': ('https://mycloud.rackspace.com/%s', ''),
      'rax-glossary': ('https://developer.rackspace.com/docs/glossary/%s', ''),
      'how-to': ('https://support.rackspace.com/how-to/%s', ''),
      'os': ('https://www.openstack.org/%s', ''),
      'os-docs': ('https://docs.openstack.org/%s', ''),
      'os-wiki': ('https://wiki.openstack.org/%s', ''),
      'git-repo': ('https://github.com/rackerlabs/'
                   'docs-core-infra-user-guide/%s', ''),
      'rackerlabs': ('https://github.com/rackerlabs/%s', ''),
      'rocket': ('https://objectrocket.com/%s', '')
  }

Linking examples
~~~~~~~~~~~~~~~~

When you reference a link using the external link library, the reference
identifier (``kc-faq``, ``rax-dev``, ``rax-devguide``) precedes the link label
and the part of the link reference that is variable as represented by the
``%s`` in the external link definition.


**Link to DRC**

.. code::

   :rax-dev:'Rackspace Developer website <>`


Note that the link element is enclosed in <>. If the element is empty, the
reference is replaced by the base url. In this example, the link reference is
replaced by ``developer.rackspace.com``.


**Link to the Docs page**

.. code::

   :rax-devdocs:`API Developer Guide <>`


**Link to a specific Dev Guide**

.. code::

   :rax-devguide:`Cloud Images Developer Guide <cloud-images/v2>`

In this example, the ``cloud-images/v2`` portion replaces the %s in the
external link definition defined in the conf.py
``http://developer.rackspace.com/docs/%s``.


**Link to API reference for a product**

.. code::

   :rax-api:`Cloud Images API Reference <cloud-images/v2>`


**Link to a API doc topic**

.. code::

   :rax-devdocs:`List images operation <cloud-images/v2/developer-guide/#list-images>`


**Link to KC article**

.. code::

   :how-to:`Getting Started with Role-Based Access Control (RBAC) <getting-started-with-role-based-access-control-rbac>`

You can see some examples of external link library references to the Rackspace
Support How To collection articles in the `Core Infrastructure User Guide
source files`_.


**Link to Glossary term**

.. code::

   :rax-glossary:`term <#term>`

You can get the glossary term links from the anchor links assigned to each term
in the published Glossary, for example the agent link is here:
https://developer.rackspace.com/docs/glossary/#agent



.. _Core Infrastructure User Guide source files: https://github.com/rackerlabs/docs-core-infra-user-guide/search?utf8=%E2%9C%93&q=%3Ahow-to


Replacing external links in your documentation source files
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Follow these instructions to update the external link library definition for
your project and update external links in your project.

#. Copy the common external link library from the `Common external link library
   definition`_.

#. Edit the Sphinx configuration file for each of your projects and replace the
   current external link library specification with the one you copied from
   the Identity project.

#. Using your text editor, do a multi-file find and replace to find all links
   to docs.rackspace.com. Then, replace the link using the external link
   reference.

   For example, replace a link to the List Images operation in Cloud Images
   API Reference on docs.rackspace.com with the following link reference:

   .. code::

      :rax-devdocs:`List images operation
      <cloud-images/v2/developer-guide/#list-images>`

#. Using your text editor, do a multi-file find and replace to find all the
   html links in your project.

   - Review each occurrence to determine whether the link can be replaced by
     an external link reference.

     For example, if you have links to a Knowledge Center article, you can
     replace it with the following link:

     .. code::

        :kc-article:`Link text <article-label>`.

     When the Sphinx project builds, the *Link text* is rendered as a link,
     and the HREF definition is populated with the full URL.

     .. code::

        http://www.rackspace.com/knowledge_center/article/TopicTitle

.. _Sphinx external link library extension: http://sphinx-doc.org/ext/extlinks.html
.. _Common external link library definition: https://github.com/rackerlabs/docs-common/blob/master/common-devguide/ext-link-library.txt
