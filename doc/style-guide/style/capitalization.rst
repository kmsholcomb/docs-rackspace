.. _capitalization:

==============
Capitalization
==============

Be judicious and consistent in your use of capitalization. Use
capitalization for proper names and proper adjectives and when it's
stylistically required. Don't use it for common nouns, for emphasis, to
attempt to give a word greater status than other words, or randomly.

This topic provides capitalization guidelines for the following items:

-  `Capitalization with
   punctuation <#capitalization-with-punctuation>`__
-  `Code <#code>`__
-  `Figures <#figures>`__
-  `Glossary terms and definitions <#glossary-terms-and-definitions>`__
-  `List items <#list-items>`__
-  `Tables <#tables>`__
-  `Terms <#terms>`__
-  `Titles and headings <#titles-and-headings>`__
-  `Variables and placeholders <#variables-and-placeholders>`__

Capitalization with punctuation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Always capitalize the first word of a new sentence. Don't start a
sentence with a case-sensitive lowercase word (such as a lowercase
command name).

Don't capitalize the word that follows a colon in a sentence, unless
the word is proper or is the beginning of a quotation.

Don't capitalize the word following an em dash, unless the word is
proper.

Code
~~~~

If you're showing sample code, follow the conventions of the
programming language used and preserve the capitalization that the
author of the code used.

Figures
~~~~~~~

Use sentence-style capitalization for figure titles, text callouts
within figures, and for legends associated with a figure.

Glossary terms and definitions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Use the following guidelines for capitalizing terms and definitions in
glossaries:

- For the glossary term, use lowercase letters unless the
  term is a proper noun or acronym. For example, use *server* instead of
  *Server*.

- For the definition, use sentence-style capitalization.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Example
   * - **token**

       An opaque string that represents an authorization to access cloud
       resources. Tokens might be revoked at any time and are valid for a
       finite duration.

For more information about formatting glossary entries and definitions,
see :ref:`glossaries`.

List items
~~~~~~~~~~

Capitalize the first letter of each list item unless the first letter
must be lowercase.

For additional guidelines about formatting lists, see :ref:`lists`.

Tables
~~~~~~

Use sentence-style capitalization for table titles, column headers,
row headers, and text in table cells.

For additional guidelines about formatting tables, see :ref:`tables`.

Terms
~~~~~

Use the following guidelines to help you decide whether a word should be
capitalized. For the correct capitalization of some common terms, see
:ref:`alphabetical-list-of-terms`.

Capitalize proper nouns and adjectives
--------------------------------------

Proper nouns and adjectives include the names of people, places,
companies, organizations, products, languages, protocols, and some
technologies, as well as trademarks.

Be aware that some of these names might have nonstandard or no
capitalization. You should always follow the capitalization that's used
by the company, shown in a dictionary, or accepted as standard in the
industry.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Examples
     -
   * - Rackspace
     - Service Advertising Protocol
   * - Hong Kong
     - WordPress
   * - Fanatical Support
     - Boolean
   * - Cloud Servers
     - OpenStack
   * - Linux
     - Internet
   * - Microsoft Windows
     - Ethernet
   * - SQL Server
     - Wi-Fi
   * - PuTTY
     - lighttpd

For the correct capitalization of Rackspace product names, see the
`Rackspace Cloud corporate website <https://www.rackspace.com/cloud>`__.

For the correct capitalization of some commonly used third-party names,
see :ref:`third-party-names-and-trademarks`.

Capitalize most acronyms, initialisms, and short forms of names
---------------------------------------------------------------

Most abbreviated forms of terms use all capitals, although exceptions
exist. Also, be aware that the corresponding spelled-out terms of
abbreviations are often not capitalized. When in doubt about the
capitalization of an abbreviation or its spelled-out term, consult a
dictionary, industry style guide, reputable website, or editor.
Following are some examples.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Abbreviation
     - Spelled out term
   * - API
     - application programming interface
   * - GB
     - gigabyte
   * - GHz
     - gigahertz
   * - I/O
     - input/output
   * - JSON
     - JavaScript Object Notation
   * - Kbps
     - kilobits per second
   * - REST
     - Representational State Transfer
   * - SaaS
     - software as a service
   * - SOA
     - service-oriented architecture
   * - WSDL
     - Web Services Description Language

For more information, see :ref:`abbreviations`.

Capitalize interface labels as they're capitalized on the interface
-------------------------------------------------------------------

When you're documenting part of the interface within a procedure or
other type of article or topic, match the capitalization used on the
interface.

However, when you use terms from the interface as common nouns, don't
capitalize the terms.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Click the action cog to the left of the check name and select **Rename
       Check**.
   * - From the Cloud Control Panel, you can rename a check.

Generally, capitalize the names of product components, systems, or utilities
----------------------------------------------------------------------------

Follow the capitalization of major component names that's established
by Marketing, Legal, and the product teams. However, be wary of
overcapitalization of product terms. Not every feature or object in a
product is a proper noun. For example, the Cloud Servers service enables
users to create a *server*, not a *Server*. When the user creates a
server, the user specifies an *image*, *flavor*, and *network*, not an
*Image*, *Flavor*, and *Network*. A Performance server has a *data disk*
and a *system disk*, not a *Data disk* and a *System disk*. A user
uses Cloud Load Balancer to create a *load balancer*, not a *Load
Balancer*.

Many terms that might be capitalized on the interface aren't
capitalized when used as common nouns. When in doubt, consult an
existing style sheet, an editor, or the product team (but be aware that
product teams sometimes tend to overcapitalize terms). Following are
some tips to help you determine whether a noun should be capitalized:

-  Generally, if you can have more than one of something, it's a common
   noun and therefore not capitalized.
-  When a common noun follows the name of a product or component,
   generally that noun isn't capitalized.
-  When you refer generally to a component, you can use lowercase (as in
   the utility or the agent).

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - Cloud Control Panel
   * - Zipit Backup Utility
   * - Rate Limiting component
   * - Cloud Identity service
   * - servers
   * - backups
   * - containers
   * - authentication

Don't capitalize common nouns
-----------------------------

Most of the time, we have no trouble determining whether a noun is
proper or common. However, we have a tendency to capitalize
product-specific terms even when they're really just being used as
common nouns. A common noun denotes a whole class of something (for
example, *servers*) or a random member of a class (for example, *a
server*). As a general rule, if you can have more than one of something,
it's a common noun and therefore not capitalized.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - You can submit up to 10 messages in a single request, but you must
       encapsulate them in a collection container (an array in JSON).
     - You can submit up to 10 Messages in a single Request, but you must
       encapsulate them in a Collection Container (an Array in JSON).
   * - Repose authentication provides caching for user tokens, roles, and
       groups.
     - Repose Authentication provides caching for User Tokens, Roles, and
       Groups.

Don't use all capitals for emphasis
-----------------------------------

To emphasize a term, show it in italics. To emphasize an important piece
of information, consider setting it apart structurally, perhaps as a
note.

Titles and headings
~~~~~~~~~~~~~~~~~~~

Use *sentence-style* capitalization for most titles and headings,
including article, chapter, table, figure, and example titles, as well as
section and procedure headings. One exception is guide titles, which use
*title-style* capitalization.

For additional guidelines for titles and headings, see
:ref:`titles-and-headings`.

.. _sentence-style-capitalization:

Guidelines for sentence-style capitalization
--------------------------------------------

In sentence-style capitalization, you capitalize only the first word of
the title or heading, plus any proper nouns, proper adjectives, and
terms that are always capitalized, such as some acronyms and
abbreviations. If the title includes a colon, capitalize the first word
that follows the colon, regardless of its part of speech.

If the heading includes text from a user interface, the capitalization
of that text must match the capitalization on the interface.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Examples
     -
   * - Preparing a cloud server to be a mail server
     - Can I buy extra IP addresses?
   * - What are cloud servers?
     - What are the PHP configuration limits for Cloud Sites?
   * - Install or upgrade PHP 5.3 for CentOS 5.x
     - How do I install my own PEAR module?
   * - Ubuntu Hardy: Using mod\_python to serve your application
     - I live outside the United States. Can I use my foreign credit card to
       pay for my account?
   * - Shopping cart software: The basics
     - Troubleshooting a Vyatta site-to-site VPN connection
   * - Back up your files
     - Differences between IMAP and POP

.. _title-style-capitalization:

Guidelines for title-style capitalization
-----------------------------------------

Title-style capitalization uses initial uppercase letters for the first,
last, and all the significant words in the title.

Capitalize all words in the title except for the following types of
words:

- Articles (*a*, *an*, *the*) unless the article is the first word in the title
  or follows a colon
- Coordinating conjunctions (*and*, *but*, *for*, *nor*, *or*, *yet*, *so*)
  unless the conjunction is the first word in the title
- Prepositions of any length, unless the preposition is the first or the last
  word in the title or is part of a verb phrase
- The word *to* in an infinitive phrase unless to is the first word in the
  title
- Second elements attached by hyphens to prefixes unless they're proper nouns
  or proper adjectives
- Words that always begin with a lowercase letter, such as literal command
  names or certain product or software names

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - Next Generation Cloud Servers Developer Guide
   * - Rackspace Cloud DNS Getting Started Guide
   * - Stand-alone Object Storage Guide
   * - Rackspace Private Cloud powered by VMware Customer Handbook
   * - Cloud Networks Release Notes

Variables and placeholders
~~~~~~~~~~~~~~~~~~~~~~~~~~

Use camelCase (for example, *userName*) unless you have to follow the
conventions of the programming language. For example, you might need to
use underscores (*user\_name*) or all capitals (*USER\_NAME*). For more
information about formatting placeholders, see :ref:`text-formatting`.
