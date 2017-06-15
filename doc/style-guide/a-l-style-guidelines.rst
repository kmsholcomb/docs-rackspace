.. _a-l-style-guidelines:

===================
A-L style reference
===================

This section of the writing style guide provides detailed guidelines
about and instructions for applying style conventions. For more
guidelines, see :ref:`m-z-style-guidelines`.

Acronyms and other abbreviations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Unless an abbreviation is common, spell out the words of the abbreviation on
the first use in an article or topic. Show the abbreviation in parentheses
after the spelled-out term; for example, access control list (ACL). On
subsequent uses in the article or topic, use the abbreviation. If you introduce
an abbreviation, use it; don't alternate between the abbreviation and the
spelled-out term.

.. note::

   In FAQ documents, treat every occurrence of a term as the first use (that
   is, spell out the term and show the abbreviation in parentheses).

Don't capitalize the spelled-out term unless it's a proper name or normally
capitalized. For example, the spelled-out term for *AJAX* is *Asynchronous
JavaScript and XML*, but the spelled-out term for *ACL* is *access control
list*.

Also use the following guidelines related to abbreviations.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Use
     - Don't use
   * - Don't show both the spelled-out term and its abbreviation in a title or
       heading. In most cases, use the abbreviation in the title or heading and
       show the spelled-out term and its abbreviation on first use in the text.
     - **Adding an ACL**

       An access control list (ACL) allows access from an outside network into
       the ObjectRocket system.
     - **Adding an access control list (ACL)**

       An ACL allows access from an outside network into the ObjectRocket
       system.
   * - Use only established abbreviations. Don't create new ones.
     - hybrid cloud
     - HC
   * - Don't use abbreviated forms of Rackspace product names.

       However, if you think that a user might use an abbreviated name in a
       search, you can tag the document with the abbreviation.
     - Cloud Block Storage
     - CBS
   * - If an abbreviation is used as part of a compound modifier, hyphenate it
       as you would a word.

       For more information about hyphenating compound modifiers, see the
       "Hyphens" section in :ref:`punctuation`.
     - 1000-bps rate
     - 1000 bps rate
   * - Don't surround abbreviations with quotation marks.
     - OS
     - "OS"
   * - Use periods only if the abbreviation normally has them (for example,
       *a.m.* and *p.m.*) or could otherwise be misread as a word, such as
       *in.* (for *inch*).
     - FAQ
     - F.A.Q.
   * - Don't use an abbreviation as a verb.
     - Use FTP to copy the file to the server.
     - FTP the file to the server.
   * - Avoid using abbreviations in the possessive. Instead, treat the
       abbreviation as an adjective or put it in a prepositional phrase.
     - Type the DBA password.

       Type the password of the DBA.
     - Type the DBA's password.
   * - To form the plural of an abbreviation, except for a unit of measure,
       append a lowercase *s* without an apostrophe.

       For most abbreviations of units of measure, the singular and plural
       forms are the same (for example, 1 pt and 10 pt).

       If an acronym already represents a plural noun, don't add an *s*.
     - user IDs

       10 mm

       FAQ
     - user ID's

       10 mms

       FAQs
   * - For abbreviated units of measure, insert a space between the number and
       the abbreviation.
     - 256 MB
     - 256MB
   * - Don't use Latin abbreviations or non-English words and phrases. For
       more information, see :ref:`avoid-obscure-words`.
     - for example
     - e.g.

Abbreviations of byte and bit
-----------------------------

*Byte* is abbreviated with an uppercase *B*. *Bit* is abbreviated with a
lowercase *b*. For example, *gigabyte* is abbreviated as *GB*, and
*gigabit* is abbreviated as *Gb*. In general, use such abbreviations
only with a number value; otherwise, spell out the term. If you want to
emphasize *bit* or *byte*, use the spelled-out term rather than or in
addition to the abbreviation.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - The 100 GB drive appears as 107.4 GB because of how the megabytes
       are counted.
   * - The unit of value for this alarm is megabits per second (Mbps).

Common abbreviations
--------------------

A common abbreviation is either an industry-standard abbreviation or one that
is well known to your target audience. Following are some common abbreviations
in the computer industry. You don't need to spell out these terms on first use,
unless you think the abbreviation is unfamiliar to your audience.

API, ASCII, BIOS, CD, CD-ROM, CGI, CLI, CPU, CSS, DNS, DVD, FAQ, FTP,
GB, GHz, GUI, GUID, HTML, HTTP, HTTPS, ID, IMAP, I/O, IP, JSON, KB, kHz,
LAN, LDAP, MB, MHz, NIC, NTFS, OLE, OS, PDF, PHP, POP, RAM, REST, ROM,
SGML, SMTP, SQL, SSL, TCP, TCP/IP, URI, URL, USB, VLAN, WAN, XML

.. _capitalization:

Capitalization
~~~~~~~~~~~~~~

Be judicious and consistent in your use of capitalization. Use
capitalization for proper names and proper adjectives and when it's
stylistically required. Don't use it for common nouns, for emphasis, to
attempt to give a word greater status than other words, or randomly.
This topic provides capitalization guidelines for the following items:

-  `Terms <#terms>`__
-  `Code <#code>`__
-  `Variables and placeholders <#variables-and-placeholders>`__
-  `Titles and headings <#titles-and-headings>`__
-  `List items <#list-items>`__
-  `Tables <#tables>`__
-  `Glossary terms and definitions <#glossary-terms-and-definitions>`__
-  `Figures <#figures>`__
-  `Capitalization with
   punctuation <#capitalization-with-punctuation>`__

Terms
-----

Use the following guidelines to help you decide whether a word should be
capitalized. For the correct capitalization of some common terms, see
:ref:`alphabetical-list-of-terms`.

-  `Capitalize proper nouns and
   adjectives <#capitalize-proper-nouns-and-adjectives>`__
-  `Capitalize most acronyms, initialisms, and short forms of
   names <#capitalize-most-acronyms-initialisms-and-short-forms-of-names>`__
-  `Capitalize interface labels as they're capitalized on the
   interface <#capitalize-interface-labels-as-they-are-capitalized-on-the-interface>`__
-  `Capitalize the names of major components, systems, or utilities
   associated with a
   product
   <#generally-capitalize-the-names-of-major-components-systems-or-utilities-associated-with-a-product>`__
-  `Don't capitalize common nouns <#do-not-capitalize-common-nouns>`__
-  `Don't use all capitals for
   emphasis <#do-not-use-all-capitals-for-emphasis>`__

Capitalize proper nouns and adjectives
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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

For more information about abbreviations, see `Acronyms and other
abbreviations <#acronyms-and-other-abbreviations>`__.

Capitalize interface labels as they're capitalized on the interface
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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

Generally, capitalize the names of major components, systems, or utilities associated with a product
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To emphasize a term, show it in italics. To emphasize an important piece
of information, consider setting it apart structurally, perhaps as a
note.

Code
----

If you're showing sample code, follow the conventions of the
programming language used and preserve the capitalization that the
author of the code used.

Variables and placeholders
--------------------------

Use camelCase (for example, *userName*) unless you have to follow the
conventions of the programming language. For example, you might need to
use underscores (*user\_name*) or all capitals (*USER\_NAME*). For more
information about formatting placeholders, see :ref:`text-formatting`.

Titles and headings
-------------------

Use *sentence-style* capitalization for most titles and headings,
including article, chapter, table, figure, and example titles, as well as
section and procedure headings. One exception is guide titles, which use
*title-style* capitalization.

For additional guidelines for titles and headings, see
:ref:`titles-and-headings`.

.. _sentence-style-capitalization:

Guidelines for sentence-style capitalization
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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

List items
----------

Capitalize the first letter of each list item unless the first letter
must be lowercase.

For additional guidelines about formatting lists, see
`Lists <#lists>`__.

Tables
------

Use sentence-style capitalization for table titles, column headers,
row headers, and text in table cells.


Glossary terms and definitions
------------------------------

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
see `Glossaries <#glossaries>`__.

Figures
-------

Use sentence-style capitalization for figure titles, text callouts
within figures, and for legends associated with a figure.

Capitalization with punctuation
-------------------------------

Always capitalize the first word of a new sentence. Don't start a
sentence with a case-sensitive lowercase word (such as a lowercase
command name).

Don't capitalize the word that follows a colon in a sentence, unless
the word is proper or is the beginning of a quotation.

Don't capitalize the word following an em dash, unless the word is
proper.

Citations
~~~~~~~~~

Occasionally you might want to include content from a third-party
source. If you do so, you must ensure that the source is reputable, the
information is accurate, the quoted material is distinguished from the
surrounding content, and the source is cited. Follow these guidelines:

-  Include content only from expert sources that have a named author or
   are from a known company. Don't quote Wikipedia articles.
-  If necessary, verify that the content is accurate.
-  Set off the quoted content from the other content in the following
   ways:

   -  If the quotation is short (just a phrase or sentence), you can
      include it in an existing paragraph. Set the quotation off with
      quotation marks, and put ending punctuation within the closing
      quotation mark.
   -  If the quotation is longer than a phrase or sentence, or it makes
      sense to separate it from the surrounding content, you can place it
      in its own paragraph. Indent the paragraph to set it off from the
      surrounding paragraphs.
   -  Don't use italics or bold to distinguish quoted content. Use such
      formatting only if it was used in the source.

-  Attribute the source as follows:

   -  If you have just one or two quotations, you can attribute them within
      the article text by stating the author, the source document, or both
      and providing a link to the source. Usually such an attribution would
      precede the quotation, as an introduction to it.
   -  If you have more than one or two quotations, follow each quotation
      with a number in square brackets. Start at [1] and number each
      quotation in the document consecutively. At the end of the document,
      use a numbered list to list each resource in the order that it's
      shown in the article. Cite the author, the name of the source, and
      provide a link to the source. Put the list under a heading such as
      “Numbered citations in this article.” Then, go back to each numbered
      reference in the article and create a link between the reference
      number (such as [1]) and the numbered item at the end of the article.

.. _cloud-account-information:

Cloud account information
~~~~~~~~~~~~~~~~~~~~~~~~~

In examples of API authentication requests, and other examples where we
are teaching the use of the API and expect that users might copy the
code and use it, use variables or the following standard values for
account numbers, user names, passwords, API keys, and so on. Format the
variables by using camelCase and italics, and also use bold within the
examples.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Information
     - Use
     - Don't use
   * - Account or tenant ID
     - *yourAccountId*

       *yourTenantId*

       ``$account``

       ``$tenant``
     - 658405
   * - User name
     - *yourUserName*

       ``$username``
     - robb4554
   * - Password
     - *yourPassword*

       ``$password``
     - J$12345\*
   * - API key
     - *yourApiKey*

       ``$apikey``
     - of938go4915e114f7ff5448910fee68c
   * - Authentication token
     - *xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx*

       ``$token``
     - 2e356864f39831523c184to646b1997b

In example API operation requests and responses, in which we want users
to see actual values from the system, use "real-looking" values that are
nevertheless obviously made up, such the following one for
``X-Auth-Token``:

.. code::

   abcdef123ghi4j5k67m8910n12op3qrs

.. warning::

   Don't include or show actual writer or user account
   credentials in code examples or screenshots.

Code examples
~~~~~~~~~~~~~

Use the following guidelines when creating blocks of code as input
or output examples:

-  Don't use screenshots to show code examples. Format them as blocks
   of code by using the appropriate markup in your authoring tool. For
   more information about formatting, see :ref:`text-formatting`.

-  When showing input, always include a command prompt (such as $).

-  As often as necessary, show input and output in separate blocks and
   provide explanations for each. For example, if the input contains
   arguments or parameters, explain those. If the user should expect
   something specific in the output, or you want to show only part of
   lengthy output, provide an explanation.

-  When the command is simple, and there's nothing specific to say
   about the output, you can show the input and output in the same code
   block, as users would actually see the code in their own terminal.
   The inclusion of the command prompt differentiates the input from
   the output.

-  Ensure that any placeholder text in code is obvious.

   - If the authoring tool allows it, apply italics to placeholders; if not,
     enclose them in angle brackets.
   - Use lowercase letters for single-word placeholders. To show multiple-word
     placeholders, don't separate the words with spaces or symbols and
     capitalize the first letter of each word after the first word (camelCase).

     .. note::

        Use Use lowercase and camelCase unless you have to follow the
        conventions of the programming language. For example, you might need to
        use underscores (account_ID) or all capitals (ACCOUNT_ID).

-  Follow the conventions of the programming language used and preserve
   the capitalization that the author of the code used.

-  For readability, you can break up long lines of input into readable
   blocks by ending each line with a backslash.

-  If the input includes a list of arguments or parameters, show the
   important or relevant ones first, and group related ones. If no other
   order makes sense, use alphabetical order. If you explain the
   arguments or parameters in text, show them in the same order that
   they appear in the code block.

The following examples illustrate many of these guidelines:

Create a VM running a Docker host
---------------------------------

#. Show all the available virtual machines (VMs) that are running
   Docker.

   .. code::

      $ docker-machine ls

   If you have not created any VMs yet, your output should look as follows:

   .. code::

      NAME ACTIVE DRIVER STATE URL

#. Create a VM that's running Docker.

   .. code::

      $ docker-machine create --driver virtualbox test

   The ``--driver`` flag indicates what type of driver the machine runs
   on. In this case, ``virtualbox`` indicates that the driver is Oracle
   VirtualBox. The final argument in the command gives the VM a name, in
   this case, ``test``.

   The output should look as follows:

   .. code::

      Creating VirtualBox VM...
      Creating SSH key...
      Starting VirtualBox VM...
      Starting VM...
      To see how to connect Docker to this machine, run:
      docker-machine env test

#. Run docker-machine ls again to see the VM that you created.

   The output should look as follows:

   .. code::

      NAME ACTIVE DRIVER STATE URL SWARM
      test virtualbox Running tcp://192.168.99.101:237

Run the application
-------------------

#. Run a container from the image. The application code uses the
   environment variables that you defined to connect to the MongoDB
   container.

   .. code::

      $ docker run --detach \
        --env MONGO_HOST=$MONGO_HOST \ env MONGO_PORT=$MONGO_PORT \ env
        --MONGO_SSL=$MONGO_SSL \ env MONGO_DATABASE=$MONGO_DATABASE \ env
        --MONGO_USER=$MONGO_USER \ env MONGO_PASSWORD=$MONGO_PASSWORD \ publish
        --5000:5000 \
        guestbook-mongo:1.0

#. View the status of the container by using the ``--latest`` parameter.

   .. code::

      $ docker ps --latest

The status of the container should begin with ``Up``.

Remove the containers already using the port
--------------------------------------------

#. To identify the containers that are using the port, run the following
   command, changing ``<port>`` to the port number that you want to use.

   .. code::

      $ docker ps -a | grep <port>/tcp

#. To remove the containers, run the following command for each
   container identified in step 1, changing ``<containerId>`` to the ID
   of the container.

   The ``--force`` argument ensures that the container is removed even
   if it's currently running.

   .. code::

      docker rm --force --volumes <containerId>

Troubleshooting
---------------

Sometimes, when you use a docker command, you receive the following
output:

.. code::

   $ docker info Get http:///var/run/docker.sock/v1.20/info: dial unix
   /var/run/docker.sock: no such file or directory.
   * Are you trying to connect to a TLS-enabled daemon without TLS?
   * Is your docker daemon up and running?

If you receive this output, your VM isn't running on a Docker host.

Contractions
~~~~~~~~~~~~

Contractions help to create a less formal tone in documentation. Common
contractions, such as *can’t* and *don’t*, are usually recognizable by
readers who are proficient in English, and such contractions don't pose
a problem for human translators.

In general, you can use the following common contractions in content where
contractions are acceptable:

-  Contractions that include the word *not*, such as *aren’t*, *can’t*,
   *didn’t*, *doesn’t*, *don’t*, *isn’t*, *wasn’t*, *weren’t*, *won’t*,
   and *wouldn’t*

   If you want to emphasize the negative, however, do *not* use such a
   contraction.

-  Contractions that include *is* or *are*, such as *it’s*, *that’s*,
   *there’s*, *they’re*, and *you’re*

   Because such contractions can be confused with possessives, ensure that your
   usage is correct.

Avoid the following types of contractions, which aren't common or can
be confusing depending on context:

-  Contractions that can be misread as other words, such as *let’s*
-  Contractions with the interrogative words *how*, *what*, *when*,
   *where*, *who*, and *why*
-  Nonstandard or obscure contractions, such as *mustn’t*, *mightn’t*,
   *should’ve*, *could’ve*, and *that’ll*
-  Contractions that combine a noun and a verb, such as in “The
   service’ll stop automatically”
-  Contractions that include a company name, product name, or trademark,
   such as in “Rackspace’s the leader in hybrid cloud”

Use contractions consistently. Avoid mixing common contractions and
spelled-out forms within the same article or set of related articles.

Copyrights
~~~~~~~~~~

For both API and How-To content, copyright statements are automatically
inserted by the system. Use the generated statement unless RackLaw gives
you other instructions.

.. _dates:

Dates
~~~~~

Dates are displayed differently in different countries, so you must use
a date format that's explicit and consistent and that global users
can't misinterpret.

Unless space is limited, always show dates in the following format:
*month day*, *year*. Always spell out the month.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - November 12, 2010
     - 12 Nov 2010

       2010-Nov-12

       12/11/10

       11/12/10

       10-11-12

.. note::

   Don't use ordinal numbers for dates. For example, don't use
   *January 1st*; use *January 1* instead.

When the month, day, and year are embedded in a sentence, use a comma
before and after the year. When only the month and year are embedded in
a sentence, omit the commas unless the syntax would ordinarily require a
comma following the year.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Any sites that are using MySQL 4 after November 1, 2011, will be
       automatically migrated to MySQL 5.
   * - The Alert Logic Security Research Team used 12 months of security event
       data captured from July 2010 through June 2011.
   * - As of September 2013, a subset of customer accounts weren't being
       billed for actual usage in comparison to their preselected SQL Server
       storage allocations.

Use an all-numeric date only in the following situations:

- Space is limited, as in a table or figure.
- You need to show a literal representation of the date as it's displayed
  in the software.

Because all-numeric dates are interpreted differently in different
countries, explain the format of a numeric date, and use a consistent
format throughout the documentation. If possible, use the ISO 8601
format, which is *yyyy*-*mm*-*dd* (for example, 2012-11-10 for November
10, 2012).

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - The value that's shown for 8/19/10 represents the average number of
       extents from data collections beginning August 19, 2010.

For information about and examples for showing a date range, see
:ref:`ranges-of-numbers`.

.. _email-addresses:

Email addresses
~~~~~~~~~~~~~~~

For example email addresses, use **example.com** or **example.org**. The
Internet Assigned Numbers Authority (IANA) reserves these domain names
for use in examples.

.. note::

   For How-To articles, don't use **kcexample.com**. Rackspace
   no longer owns this domain name. Use **example.com** or **example.org**
   instead.

Format example email addresses as bold. For example,
**yourName@example.com**.

If you document an actual email address, use the convention in your
authoring environment to make the email address live.

File types
~~~~~~~~~~

For references to a file type in text (not code), use one of the
following naming conventions, depending on the type of file and the
context:

-  Generic name, such as an initialization file or a configuration file
-  Standard abbreviation, such as a PDF file or an XML file
-  File name extension, such as a .zip file

Use a generic name or a standard abbreviation if one exists. If a
generic name or a standard abbreviation doesn't exist or isn't
appropriate given the context, use the file name extension. The
following table provides some common file types and guidelines for
referring to them.

.. list-table::
   :widths: 20 40 40
   :header-rows: 1

   * - File type
     - Guideline
     - Example
   * - configuration
     - Use the term *configuration* unless you're naming a specific file.
     - The main logrotate configuration file is located at
       ``/etc/logrotate.conf.``
   * - HTML
     - Use the term *HTML* unless you're naming a specific file.
     - From the website, you can access HTML files.

       The frequently asked questions are located in the **faq.htm** file.
   * - initialization
     - Use the term *initialization* unless you're naming a specific file.
     - The initialization files contain default parameter values.

       Copy the **calibrate.ini** file.
   * - JSON
     - Use the term *JSON* unless you're naming a specific file.
     - You can directly edit the JSON environment file to add attributes
       specific to your configuration.

       The parameters provided with ``/type=install`` are visible in the
       **bootstrap.json** file.
   * - XML
     - Use the term *XML* unless you're naming a specific file.
     - The file is an XML document that defines configuration information
       regarding the web application.

       A service name maps to a collection of configuration entries in the
       Hadoop **core-site.xml** file.
   * - zip
     - Use the term *zip* for both general and specific references.
     - In the example, **file.zip** is the name that you assign to the zip
       file.

Glossaries
~~~~~~~~~~

Create a glossary to document the following items:

-  New, unfamiliar, or unique terms
-  Familiar terms used in a new or special way
-  Abbreviations or acronyms that should be clarified

This section provides guidelines for the following items:

- `Glossary terms <#glossary-terms>`__
- `Glossary definitions <#glossary-definitions>`__
- `Cross-references to glossary terms <#cross-references-to-glossary-terms>`__
- `Guidelines for a comprehensive glossary
  <#guidelines-for-a-comprehensive-glossary>`__

Glossary terms
--------------

To show the glossary term that you're defining, use the following
guidelines:

- Use the singular form unless the term is always plural. For example, use
  *server* instead of *servers*.
- Use lowercase letters unless the term is a proper noun or acronym. For
  example, use *server* instead of *Server*.
- If the term has an acronym or abbreviation, show the term either in its
  spelled-out form or shortened form, depending on which term is more familiar
  to users. If you use the spelled-out form, follow it with the abbreviation in
  parentheses.

To alphabetize glossary terms, use the word-by-word method. In this
method, terms that contain more than one word separated by spaces or
commas are alphabetized by the first word only, unless the first word of
two or more entries is the same. In that case, the second and subsequent
words are used to determine the alphabetical order. Hyphens, slashes,
and apostrophes continue a single word.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Example word-by-word alphabetization
   * - new math

       newborn

       new/old

       newspaper

Glossary definitions
--------------------

Make your glossary definitions brief. Try to restrict definitions to no
more than one or two short paragraphs, and avoid the inclusion of notes
or tips. If your definition is longer than one or two short paragraphs,
it might be more appropriate as a concept in an overview section rather
than in a glossary.

Begin the definition with a descriptive phrase. Capitalize the first
letter of the phrase, and end the phrase with a period. Follow the
initial phrase with one or more sentences as needed.

How you begin the definition also depends on what part of speech the
term is:

-  **Noun**: Begin with the appropriate article (a, an, or the) and a
   noun phrase.
-  **Verb**: Begin with the infinitive form of another verb that defines
   the term.
-  **Adjective**: Begin with a verb such as describes or pertains to.
-  **Abbreviation**: Begin with the spelled-out term.

The following table shows examples.

.. note::

   In a comprehensive glossary, you might need to start the
   definition with a qualifier that identifies the service to which the
   term relates. For more information, see `Guidelines for a comprehensive
   glossary <#guidelines-for-a-comprehensive-glossary>`__.

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Type
     - Example
   * - Noun
     - **token**

       An opaque string that represents an authorization to access cloud
       resources. Tokens might be revoked at any time and are valid for a
       finite duration.
   * - Verb
     - **resize**

       To convert an existing server to a different flavor, in essence, scaling
       the server up or down. The original server is saved for a period of time
       to allow rollback if a problem occurs.
   * - Adjective
     - **RESTful**

       Describes a kind of web service API that uses REST.
   * - Abbreviation
     - **API**

       Application Programming Interface. A set of commands, functions, and
       protocols that programmers can use to create application services by
       using an open application.

Cross-references to glossary terms
----------------------------------

Use the following guidelines when creating cross-references within a
glossary:

-  For a term with a definition located under a different entry, use a
   *See* entry in place of the definition.

-  For a term with a definition that's related to, is similar to, or
   contrasts with another term, refer to the term in one of the
   following ways. If that term actually occurs in the definition, you
   can simply link to its definition from the term. If the term doesn't
   occur in the definition, add a *See also* entry at the end of the
   definition.

   **Tip:** To highlight a difference between two terms, you can use a
   *Contrast with* entry.

-  Format the cross-reference as follows:

   -  If using a *See* or *See also* reference, type *See* or *See also*,
      and apply italics. If you're referring to more than one item,
      italicize *and*.

   -  Make the term a link to the cross-referenced term.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - **address**

       See address space.
   * - **collection**

       A group of packages that have the same qualifier.
   * - **data point**

       A value that stores metrics. Metrics are stored as full resolution data
       points, which are periodically rolled up (condensed) into coarser data
       points. *See also* data granularity.
   * - **replace**

       To recover by dropping the selected database and re-creating it.
       *Contrast with* copy over.

Guidelines for a comprehensive glossary
---------------------------------------

A comprehensive glossary might have the following types of terms:

-  Industry-standard terms
-  Third-party product terms
-  Rackspace-specific terms that apply to only one service
-  Rackspace-specific terms that are general or apply to many different
   services
-  Rackspace-specific terms that apply to two or more services and have
   different meanings for two or more services

Following are guidelines for how to handle each type of term in the
comprehensive glossary:

-  Include industry-standard terms only if they're integral to
   understanding how a Rackspace service works. However, don't include
   terms that are well-known or common (such as *browser* and *blog*).
   In the definition, describe how Rackspace incorporates the idea
   represented by the term, or which service employs it. For example,
   *API*.

-  Avoid including third-party terms. Within the documentation itself,
   provide links to third-party websites if you want to provide more
   information about third-party terms. A Rackspace glossary should
   contain mainly Rackspace terms. If the user could find the meaning
   outside of a Rackspace document by using a browser search, then we
   probably don’t need to include it in the glossary. For example,
   *Apache*.

-  If a term is specific to one Rackspace service, start the definition
   with the name of that service in parentheses, and italicize it.

-  If a term is general or applies to many different services, you do
   not need to qualify it.

-  If a term is specific to more than one service but has a different
   meaning for each service, provide all the relevant definitions in one
   glossary entry. Place each definition in a separate paragraph and
   start the definition with the service name, in parentheses and
   italicized.

IP addresses
~~~~~~~~~~~~

An *IP address* uses a sequence of numbers to uniquely identify a
particular computer on the Internet.

When you're discussing IP addresses or referring to a specific IP
address, don't use *IP* only; use *IP address*. You don't need to
spell out *IP* on first use.

When you need to refer to a specific version of the IP, use *IPv4
address* or *IPv6 address* as appropriate.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - If your website is hosted in the DFW data center, you can use the
       following primary and secondary IP addresses:

       • Primary: 74.205.61.228

       • Secondary: 74.205.61.229

       • Additional: 72.32.36.144/28 (72.32.36.145 - 72.32.36.158)
   * - Each Vyatta appliance is assigned one public IPv4 address.
   * - If you're using IPv6 on your server, you might need to add the IPv6
       addresses of your name servers to the **resolv.conf** file.

If you need to show an example IP address, don't use one that's or
might be assigned to a computer. Instead, use one that's globally
defined for documentation. Valid IPv4 address blocks are provided in
`RFC5737 <https://tools.ietf.org/html/rfc5737>`__, and a valid IPv6
prefix is provided in `RFC 3849 <http://tools.ietf.org/html/rfc3849>`__.

Keyboard keys
~~~~~~~~~~~~~

Different keyboards use different names for common keys. For
consistency, use the following key names unless the technology that you
are documenting requires other forms:

-  Alt
-  arrow keys (generic)
-  Backspace
-  Command
-  Ctrl
-  Del
-  Down Arrow
-  End
-  Enter
-  Esc
-  Home
-  Ins
-  Left Arrow
-  Option
-  Page Down
-  Page Up
-  Right Arrow
-  Shift
-  Space
-  Tab
-  Up Arrow

When showing specific key names and key combinations, apply bold and use
the following guidelines:

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - When telling users to *type* a letter key (as in a command), use
       lowercase for the letter unless uppercase is required. Use *type* or
       *enter* when the action results in output on the interface.
     - When prompted, type ``y`` and then press **Enter**.

       To change from command mode to insert mode, type ``i``.
   * - When telling users to press a letter key (as in a key combination),
       capitalize the letter. Use press when the action doesn't result in output
       on the interface.

       **Note**: Don't use the verbs *hit*, *strike*, or *punch*.

       Separate the key names by **-** or **+**, depending on whether you're
       documenting Linux or Windows. If you're documenting for both, pick one
       symbol and use it consistently.
     - When you're finished, press **Ctrl+X** to exit, type ``y`` to confirm
       your changes, and then press **Enter** to save as the indicated file.

       Press **F3** to find the next matching process, or press **Esc** to quit
       the search.

       To move forward word by word, press **W**. To move back word by word,
       press **B**.
   * - Avoid using *key* with specific key names.

       If needed for clarity, on the first use of a key name, you can use the
       definite article *the* and *key* with the name. On subsequent uses,
       refer to the key only by its name.
     - Press **F3** to find the next matching process, or press **Esc** to quit
       the search.

       Press the Help key (**F1**).
   * - To show a key combination, use a plus sign between the names of the
       keys.
     - To toggle between the progress bar screen and a Linux TTY screen, press
       **Ctrl+Alt+F2**.
   * - If part of a key combination requires the use of the **Shift** key (such
       as typing an asterisk or an uppercase letter), add **Shift** to the
       combination and then provide the name or symbol that results from
       pressing **Shift** (such as \*\*\*\*\* or **P**).
     - To jump to the end of the file, press **Shift+G**.

       To apply the general number format, press **Ctrl+Shift+~**.

.. _links-and-cross-references:

Links and cross-references
~~~~~~~~~~~~~~~~~~~~~~~~~~

Use cross-references to help users navigate content and find content
that's related to what they're currently viewing. Cross-references can
be linked or not linked, depending on the location of the content to
which you're referring.

-  When you refer to content within the same article or section, such as
   tables, figures, examples, or a subsection, create a simple textual
   cross-reference that isn't linked.

   .. note::

      Users typically expect links to take them to a location outside of the
      article or section that they're currently reading, so links that just
      jump to another place in the same article or section can be confusing.
      Exceptions are a TOC, or *jump list*, at the top of an article or section
      that provides links to the high-level headings in the article or section,
      and "back to top" links that take the user back to the top of the page.

-  When you refer to other content, whether created by Rackspace or outside of
   Rackspace, provide a link to that content. Ensure that the link is active
   and that the content is up-to-date. Periodically check the link and content.

Use the following guidelines to create clear and specific cross-references and
links. For examples, see the table at the end of the topic.

- Begin a cross-reference sentence by explaining the purpose or benefit of the
  cross-reference (such as more information or examples). Such context helps
  users decide whether to follow the reference.

- Use *information about* rather than *information on*.

- Use *preceding* and *following* to locate information in an article or topic.
  Don't use *above*, *below*, *earlier*, or *later*.

- Ensure that the text of a link sufficiently describes the destination
  content.

  - For links at the end of an article or topic that point to related
    information or to a next step, use the title of or a heading in the
    destination content as the link text.
  - When links are inline, use about three or four words of existing text as
    the link text. Choose words that best describe the destination content.
  - If existing text can't sufficiently describe the destination content,
    create a cross-reference sentence for the link. For the link text, use the
    title of or a heading in the destination content, if possible. Avoid
    providing an actual URL, unless you think that having the URL is helpful
    for the user.
  - Don't provide links from ambiguous phrases such as *Click here* or
    *More information*.

  .. note::

     Provide links *inline* only when it's necessary or helpful for the
     user to follow the link to understand the current topic or complete the
     task. Provide links to related but not essential information, and to
     next steps, at the end of the article or section.

- If a link points to a location other than the current site (for example, out
  of the Support website or away from developer.rackspace.com), provide context
  that describes the location.

- Don't code a link to open in a new tab or window. Users can choose whether
  they want open a link in a new tab or window.

- If your article or topic has multiple subheadings, provide a TOC (jump list)
  at the beginning of the article or topic, after an introduction. Use the
  heading text as the link text, and typically link only to the top-level
  headings in the article or topic.

  .. note::

     If the UI automatically builds a TOC or jump list for the article, don't
     duplicate it by creating one manually within the article.

- Don't use quotation marks around link text.

- Create and format links according to the authoring tool that you're using.
  Test links to ensure that they're live and that they point to the correct
  destination.

- Don't link to information more than once in an article or topic.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - For more information about the protocols that you can choose when
       configuring a load balancer, see `Available protocols when configuring a
       Cloud Load Balancer <https://support.rackspace.com/how-to/available-protocols-when-configuring-a-cloud-load-balancer/>`__.
     - See `Available protocols when configuring a
       Cloud Load Balancer <https://support.rackspace.com/how-to/available-protocols-when-configuring-a-cloud-load-balancer/>`__
       for more information about the protocols that you can choose when
       configuring a load balancer.
   * - Snapshots are described in `Create and use Cloud Block Storage
       snapshots <https://support.rackspace.com/how-to/create-and-use-cloud-block-storage-snapshots/>`__.
     - Snapshots are described `later in this Getting Started Guide <https://support.rackspace.com/how-to/create-and-use-cloud-block-storage-snapshots/>`__.
   * - The following table lists the OpenStack versions and components
       supported by the current releases of Rackspace Private Cloud.
     - The table below lists the OpenStack versions and components supported by
       the current releases of Rackspace Private Cloud.
   * - The most current versions of all SDKs are located on the
       `Rackspace Developer Docs site <https://developer.rackspace.com/docs/#sdks>`__.
     - The most current versions of all SDKs are located on the Rackspace
       Developer Docs site: https://developer.rackspace.com/docs/#sdks.
   * - You can obtain the key by logging in to the `Cloud Control Panel <https://mycloud.rackspace.com/>`__
       and selecting **Account Settings** from the **yourAccount** menu in the
       top-right corner of the window.
     - You can obtain the key from the Cloud Control Panel by selecting
       **Account Settings** from the **yourAccount** menu in the top-right
       corner of the window. (Log in at https://mycloud.rackspace.com/.)
   * - If you want your additional storage to be more portable or you need to
       be able to take data snapshots, consider `adding one or more volumes <https://support.rackspace.com/how-to/create-and-attach-a-cloud-block-storage-volume/>`__
       to the new server.
     - If you want your additional storage to be more portable or you need to
       be able to take data snapshots, consider adding one or volumes to the
       new server. See `Create and attach a Cloud Block Storage volume <https://support.rackspace.com/how-to/create-and-attach-a-cloud-block-storage-volume/>`__.
   * - Set the transmit rate for **Warning** and **Critical State**. (For more
       information about transmit rates, see `Rackspace Monitoring checks
       and alarms <https://support.rackspace.com/how-to/rackspace-monitoring-checks-and-alarms/>`__.)
     - Set the transmit rate for **Warning** and **Critical State**. (For more
       information about what this means, click `here <https://support.rackspace.com/how-to/rackspace-monitoring-checks-and-alarms/>`__.)
   * - If you need assistance opening the web console, see `Start a Console
       session <https://support.rackspace.com/how-to/start-a-console-session/>`__.
     - If you need assistance opening the web console, see `this article <https://support.rackspace.com/how-to/start-a-console-session/>`__.
   * - Download PuTTY from the `PuTTY website <http://www.chiark.greenend.org.uk/~sgtatham/putty/>`__.
     - `Download <http://www.chiark.greenend.org.uk/~sgtatham/putty/>`__ PuTTY.
   * - For more information about cross-domain XML files, read the
       `Cross-domain policy file specification <http://www.adobe.com/devnet/articles/crossdomain_policy_file_spec.html>`__
       article on the Adobe website.
     - For more information about cross-domain XML files, go to `Adobe's
       website <http://www.adobe.com/devnet/articles/crossdomain_policy_file_spec.html>`__.

Lists
~~~~~

The following types of lists are commonly used in documentation:

- **Ordered lists**, which are numbered. The list items must be performed or
  considered in a particular order.
- **Unordered lists**, which are delineated by bullets (and therefore also
  referred to as bullet lists). The order of the list items isn't important.

This topic provides the following guidelines for lists:

-  `Writing introductory text for
   lists <#writing-introductory-text-for-lists>`__
-  `Writing list items <#writing-list-items>`__

Writing introductory text for lists
-----------------------------------

Provide context for a list by introducing it. In most cases, you use a
sentence; however, you can introduce procedures with a heading. Use the
following guidelines when introducing lists.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - Introduce a list with a sentence, and end the sentence with a colon. If
       another sentence intervenes between the introductory sentence and the
       list, end the introductory sentence with a period instead of a colon.

       **Note**: Avoid using fragments to introduce lists. Fragments can be
       harder to understand than sentences.

     - You can use this product to perform the following tasks:

       You can use this product to perform the following tasks. You must
       extract objects from the database to complete these tasks.
   * - For a partial list only, use the verb *include* in the introductory
       text.
     - The directory includes the following files:

       (*Includes* is correct only if you're listing some, but not all, files
       in the directory.)
   * - Don't quantify items in introductory text. Quantifying items could
       cause an error if the list changes.
     - *Use:*

       The following methods are available:

       *Don't use:*

       The following three methods are available:
   * - Don’t tell users to "do the following." The verb *do* is weak, using
       *following* as a noun in this context is incorrect, and the whole phrase
       is ambiguous.

       Use a stronger and more meaningful verb. Use *following* only as an
       adjective, unless you're referring to an entourage, posse, retinue, or
       group of fans. Ensure that the introduction to a list provides enough
       context for users to understand what information the list is providing.
     - *Use:*

       You can use this product to perform the following tasks:

       The following methods are available:

       *Don't use:*

       You can use this product to do the following:

       The following are available:

.. _writing-list-items:

Writing list items
------------------

Use the following guidelines when writing list items:

-  Capitalize the first letter of each list item unless the first letter
   must be lowercase.
-  Make all list items parallel. For example, all items start with
   fragments, or all items use sentences. A list can have a mix of
   fragments and sentences as long as all of the items start with a
   fragment.
-  Punctuate list items as follows:

   -  In a list of only sentences, including imperative statements, use
      punctuation at the end of each item.
   -  In a list of only fragments, use no punctuation at the end of each
      item.
   -  In a list of fragments, some or all of which are followed by
      sentences, use punctuation at the end of every fragment and sentence
      in the list.

-  Don't connect separate list items with commas or conjunctions
   (*and*, *or*).

-  Avoid using articles (*a*, *an*, *the*) to start list items.

-  When a list provides a series of terms or phrases and then more
   information about them, format the list as follows:

   -  Show the term or phrase in bold. Using bold makes the list easier to
      scan.
   -  If you need to separate the initial term or phrase from the
      information that follows it, use a colon. However, if you don't need
      a separator, don't use one. (For an example of a list in which
      separators aren't necessary, see the list at the top of this topic.)

-  Unless another order makes sense or is preferable, alphabetize list
   items.

The following sections show examples of the indicated types of lists.

All list items are sentences, example
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When you create an isolated network, the following limitations apply:

- The isolated network must exist in the same region as the server.
- You can create up to three isolated networks with up to 64 servers attached
  to each one.
- After you create an isolated network, you can't rename it.

All list items are fragments, example
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The example creates a database instance called myrackinstance with the
following characteristics:

- 512 MB instance flavor
- Volume size of 2 GB
- Database named ``sampledb`` with a ``utf8`` character set and a
  ``utf8_general_ci`` collation - User named ``simplestUser`` with the password
  ``password``

All list items are imperative statements, example
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You can use Cloud Backup to perform the following actions:

- Select the files and folders from your server that you want to back up.
- Run your backups manually or on a schedule.
- See the activity from all your backups.
- Use AES-256 encryption with a private encryption key that only you know.
- Restore individual files and folders from a particular date.
- Save space with incremental backups that save only the changed portions of
  files.
- Create unlimited backups.

List items mix fragments and sentences, example
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

To run the examples in this guide, the following prerequisites are
required:

- Rackspace Cloud account. To sign up for a Rackspace Cloud account, go to the
  Rackspace Public Cloud signup page.
- Rackspace user name and password that you specified during registration.

List that provides terms and more information, example
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You have the following choices for your virtual IP:

- **Public**: This setting allows any two servers with public IP addresses to
  be load balanced. These can be nodes outside of the Rackspace network, but if
  they are, standard bandwidth rates apply.
- **Shared Virtual IP**: Use this setting if you want to load-balance multiple
  services on different ports while using the same virtual IP address.
- **Private Rackspace network**: This is the best option for load-balancing two
  Cloud Servers because it allows the load-balancing traffic to run on the
  Rackspace Cloud internal network, called ServiceNet. This option has two
  distinct advantages: the rate limit is double what the rate limit is on the
  public interface, and all traffic on the ServiceNet between Cloud Servers is
  not charged for bandwidth.
