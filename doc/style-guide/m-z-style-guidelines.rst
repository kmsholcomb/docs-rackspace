.. _m-z-style-guidelines:

===================
M-Z style reference
===================

This section of the writing style guide provides detailed guidelines
about and instructions for applying style conventions. For more
guidelines, see :ref:`a-l-style-guidelines`.

Messages
~~~~~~~~

If you help write the message text for a product or you suggest edits to
message text, use the guidelines in this topic.

.. note::

   Change message text *only* at the request of (or as a
   suggestion to) the developer. When citing message text in a document,
   cite the text that the user sees in the product.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Example
     - Comments
   * - Use complete sentences, when possible.
     - *Use:*

       The authentication token isn't valid.

       *Avoid:*

       Invalid authentication token
     - Include articles (*a*, *an*, *the*) to make the sentence complete. If
       possible, use active voice.

       **Note**: Message text that serves as a heading or label (such as
       ``Elapsed:hh:mm:ss``, which indicates elapsed time) is acceptable as
       a fragment.
   * - Use more than one sentence if required for clarity.
     - You must provide a name for each domain. null isn't a valid domain
       name.
     - Write brief and simple sentences that clearly state the problem.
       Separate the sentences with a period (or question mark, if applicable),
       not with a semicolon.
   * - Avoid using only uppercase letters.
     - *Use:*

       The requested image $UUID has automatic disk resizing disabled.

       *Avoid:*

       THE REQUESTED IMAGE $UUID HAS AUTOMATIC DISK RESIZING DISABLED.
     - Lines with excessive capitalization are hard to read. Use all uppercase
       letters only for words that require it, such as a keyword, a data type,
       or a specific table name that's displayed in all uppercase letters to a
       database user.
   * - When possible, include a recommendation, either a potential fix or a
       reference to a document for more information.
     - The system is out of virtual IP addresses. Contact Support so they can
       allocate more virtual IP addresses.

       The value -1.0 can't be accepted. Specify a positive integer value for
       the volume size.
     - Messages should provide specific information about how the user should
       continue.
   * - Be specific.
     - *Use:*

       The live migration of instance 89a5e582-d3f3-4665-ate2-03c2114f0bib to
       host compute2 failed.

       *Avoid:*

       Live migration failed.
     - Messages should provide as much detailed information as possible.
   * - Use *n* to represent an unspecified or generic number. Use *x* to
       represent an unknown version number.
     - The rate limit has been reached (*n* requests in 24 hours). Please try
       again later.

       This option is available only for Ubuntu 12.\ *x*.
     - None
   * - Avoid blaming the user.
     - *Use:*

       The request couldn't be understood by the server because of malformed
       syntax.

       *Avoid:*

       You entered bad request syntax.
     - Rewrite messages that imply fault on the part of the user. Use passive
       voice when necessary.
   * - When possible, use positive statements.
     - *Use:*

       The given limit must be positive and must be less than 50.

       *Avoid:*

       The given limit can't be negative and can't be greater than 50.
     - Positive statements are easier to understand than negative statements.

Names
~~~~~

Don't use real or copyrighted names in examples. For example, don't
use john.smith@example.com.

See the following topics for information about product names:

- `Product names and version number <#product-names-and-version-numbers>`__
- :ref:`third-party-names-and-trademarks`

Notes and other notation types
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Notations (notes, tips, and warnings) call out important or helpful
information. Use them sparingly, according to the guidelines in the
following table.

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Notation type
     - Description
   * - Important
     - Presents an important or essential point. As a rule, users must pay
       attention to important notations to complete a task or understand a
       topic.
   * - Note
     - Provides information that emphasizes or supplements information in the
       text. A note can provide information that applies only in certain cases.
   * - Tip
     - Provides useful information that might improve product performance or
       make procedures easier to follow. Tips provide the following benefits:

       • Help users learn techniques or procedures
       • Show alternative ways of doing something
       • Provide shortcuts
       • Provide helpful (but not essential) information

   * - Warning
     - Alerts users to potential hazards or highlights critical
       information. Use a warning for situations in which users could lose
       data, compromise data integrity, or disrupt operations if they don't
       follow instructions carefully.

When creating notations, use the following guidelines:

-  Use the style or element in your authoring tool to create the
   notation. If there is no style or element, create the notation as
   follows: Type the word **Important**, **Note**, **Tip**, or
   **Warning**, make the word bold, follow it with a colon, and then provide
   the text of the notation in regular font. If a notation contains more than
   one item (such as two notes presented in a unordered list), make the label
   plural (for example, **Notes**).

-  Place a notation as close as possible to the information that it
   emphasizes or clarifies.

-  Don't "stack" notations of the same type (for example, by following
   one labeled note directly with another labeled note). Instead, use
   separate paragraphs or an unordered list within a single notation. It
   is acceptable for notations of different types to follow one another.

Numbers
~~~~~~~

Use the following guidelines for showing numbers in documentation.

-  `Numbers versus words <#numbers-versus-words>`__
-  `Commas in numbers <#commas-in-numbers>`__
-  `Ranges of numbers <#ranges-of-numbers>`__
-  `Unspecified, generic, and unknown
   numbers <#unspecified-generic-and-unknown-numbers>`__

Numbers versus words
--------------------

Spell out numbers from zero through nine, except in the cases shown in
the following table. In these cases, or if the number is 10 or larger,
use numerals.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Exception
     - Example
   * - Numbers as they're displayed
     - The returned value is 0.
   * - Numbers to use as input
     - Type **1** and press **Enter**.
   * - Series of the same type of items where at least one of the numbers is
       greater than nine
     - Unit A requires 5 nodes, Unit B requires 17 nodes, and Unit C requires 9
       nodes.
   * - Numbers with symbols
     - 7%
   * - Numbers with units of measure or abbreviations
     - 5 mm, 3-inch disk
   * - Numbers that indicate dimensions
     - 8x8 feet
   * - Time
     - 5:45 p.m.

Avoid beginning a sentence with a number. If you must begin a sentence
with a number, spell out the number unless the number is part of a
product, service, or company name.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Ten vendors, including Rackspace, were assessed based on the following
       attributes:

       451 Research applied a weighting system to highlight the attributes that
       are most valued by end users.

Don't use the spelled-out form of a number followed by a numeral in
parentheses. However, if you think that a user might misread the numeral
0 as the letter O, you can clarify by spelling out zero parenthetically
after the numeral.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - two panels

       zero probability

       Enter **0** (zero). *(acceptable)*
     - two (2) panels

       zero (0) probability

.. _commas-in-numbers:

Commas in numbers
-----------------

Use commas in numbers with five or more digits. However, don't use
commas in the following types of numbers:

- Addresses
- Fractional part of a decimal number
- Page numbers
- Literal representations of user-entered values or displayed values

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - 9001 N IH 35

       1452.7532

       page 1055

       1024 bytes
     - 9,001 N IH 35

       1,452.753,2

       page 1,055

       1,024 bytes

.. note::

   Don't use European-style numbering, which uses commas in the
   place of periods. For example, use 3.14159, not 3,14159.

.. _ranges-of-numbers:

Ranges of numbers
-----------------

When describing number ranges, use the following guidelines:

- To describe an inclusive range, use *through*. When space is limited, use an
  en dash instead. Don't use the word *inclusive* in your description.

- Use prepositions as follows:

  - If you use *between* to introduce a range, use *and* to conclude the
    range. Using *between* and *and* implies a noninclusive range.
  - If you use *from* to introduce a range, use *through* or *to* to
    conclude the range.
  - Don't mix *between* or *from* with an en dash.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - step 12 through step 16
       options 11–15 *(limited space)*
       any value from 1 through 258
     - step 12 through step 16, inclusive
   * - from 10 to 20 diagrams
     - from 10–20 diagrams
   * - between 2010 and 2012
     - between 2000–2002

Unspecified, generic, and unknown numbers
-----------------------------------------

To represent an unspecified or generic number, use *n* as the variable
and apply italics.

To represent an unspecified or unknown version number, use *x* for each
digit and apply italics.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - Move the insertion point *n* spaces to the right.

       Select the **Use n I/O Sessions** check box.

       Your BlackBerry software must be version 4.\ *x*.

Parameters
~~~~~~~~~~

When documenting parameters, use the following guidelines:

-  In request and response examples, show all of the parameters.

-  Describe all of the parameters in tables preceding the examples.
   Use the following guidelines for writing descriptions:

   -  Provide meaningful information about the parameter; don't just repeat
      the parameter's name. Link to other sections of the documentation if
      more explanation is needed or if the list of possible values is long.

   -  Write the first sentence of a description with an implied subject.
      For example, if the parameter is ``name``, the description might be
      "Server name, which becomes the initial host name of the server."

   -  Include any valid values and default value at the end of the
      description. Use the formats "Valid values are *n* and *n*." and "The
      default is *n*." For example, "Valid values are ``true`` and
      ``false``." and "The default is ``false``."

-  For request body parameters only, label the required parameters by
   adding the *(Required)* qualifier to the beginning of the
   description. For example:

   *(Required)* Path of the parameter to update. Valid values are
   ``/enabled``, ``/vault/region``, ``/vault/use_internal``, and
   ``/log-level``.

   Don't label optional request body parameters. Also, don't label URI,
   query, or response body parameters as either optional or required.

-  When listing and describing request and response body parameters in
   tables, show the parameters in the same order as they're shown in
   the examples. If you have more than one example, match the order in
   the first example shown.

-  Format parameter names in text according to the guidelines in `Text
   formatting <#text-formatting>`__.

.. _placeholder-text:

Placeholder (variable) text
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Placeholder text (also referred to as variable text or replaceable text)
stands for an object whose specific name is unknown to us. Placeholders
are included when documenting syntax for how a command or path should be
constructed. Users supply the relevant value for the placeholder
when using the command or syntax.

Placeholder text usually indicates the type of element that's being
represented. For example, *directoryName* would likely indicate the name
of a directory.

.. note::

   Placeholder text is distinct from *environment variables*.
   Environment variables have established formats and names, such as
   ``$account``, and their values are set in the system by users and
   used consistently. By contrast, a placeholder is given a relevant value
   by the user at the time that the user runs the code or types the
   path. For information about formatting environment variables, see `Text
   formatting <#text-formatting>`__.

When creating placeholder text, use the following guidelines.

.. note::

   For specific information about showing placeholders for
   account information such as account numbers, user names, passwords, and
   API keys, see :ref:`cloud-account-information`.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guidelines
     - Example
   * - Within regular text, show placeholder text in italics.

       Within code samples, use the RST ``:samp:`` directive, and enclose the
       placeholder text in curly braces. This formatting renders the
       placeholder in italics.

       If you can't apply text formatting to the code, enclose placeholders in
       punctuation that doesn't have any other special use in the code. For
       example, use angle brackets or curly braces. Use a consistent convention
       throughout the documentation set.
     - :samp:`nova boot {serverName} --image {image} --flavor {flavor} --nic
       net-id=net1_id`
   * - Use lowercase letters except when showing a multiple-word placeholder.

       To show a multiple-word placeholder, don't separate the words with
       spaces or symbols. To distinguish the words in the placeholder,
       capitalize the first letter of each word after the first word (called
       camelCase). Don't capitalize the first word.

       **Note**: Use lowercase and camelCase unless you have to follow the
       conventions of the programming language. For example, you might need
       to use underscores (account_ID) or all capitals (ACCOUNT_ID).
     - *password* *serverName* *apiKey* *tenantId*
   * - In general, use one or more whole words to represent a placeholder.
       Don't sacrifice clarity for brevity. Create placeholders that are
       descriptive and meaningful.
     - *device* (instead of *dev*)

       *installationDirectory* (instead of *installDir*)

       *mode* (instead of *########*)

When explaining a placeholder, use the following guidelines.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guidelines
     - Example
   * - Avoid stand-alone clauses that begin with *where*. Instead, use a
       sentence.
     - *Use:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       *yourAccountId* is your actual account number, which is returned as part
       of the authentication service response.

       *Avoid:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       where *yourAccountId* is your actual account number, which is returned
       as part of the authentication service response.
   * - If you need to explain two or more placeholders, use an unordered list.
     - From a supported web browser, type the following URL:

       **http://hostName:portNumber/ed/index.html**

       The placeholders in the URL are defined as follows:

       • *hostName* is the name of the host computer on which the application
         server is installed.

       • *portNumber* is the port number assigned to the application server.
         The default is 8082.
   * - Show the placeholder in regular text with the same formatting that it's
       shown in the path or code. For example, if you can show it in italics,
       use italics when explaining it. If you first show the placeholder in a
       code block and need to enclose it in angle brackets, show it in angle
       brackets and monospace when explaining it.
     - *Use:*

       **https://dfw.bigdata.api.rackspacecloud.com/v1.0/yourAccountId/**

       *yourAccountId* is your actual account number, which is returned as part
       of the authentication service response.

       *Use:*

       Run the following command, replacing ``<dockerHostName>`` with the name
       of your Docker host:

       ``docker-machine env <dockerHostName> --shell cmd``

Plurals
~~~~~~~

Use the following general guidelines for forming and using plurals. To
find out how to form the plural of a particular word, or for information
about whether to use the singular or plural form of a particular word,
see :ref:`alphabetical-list-of-terms` or consult a dictionary.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - To form the plural of an abbreviation, an acronym, or a number, add a
       lowercase *s* without an apostrophe.

       If an acronym already represents a plural noun, don't add an *s*.

       **Note**: To refer to more than one FAQ document or section, add the
       appropriate noun after *FAQ* and make the noun plural—for example,
       *FAQ articles*. Follow this guideline for other plural acronyms when
       you need to refer to more than one instance of them.

     - CPUs, APIs, IDs, OSs, the 1990s, 0s and 1s

       frequently asked questions (FAQ)
   * - To form the plural of a single letter or a symbol, add an apostrophe and
       a lowercase *s*.
     - x's, #'s
   * - Abbreviated units of measure are both singular and plural; no *s* is
       necessary.
     - 5 mm, 20 in., 20 min
   * - Don't use *(s)*, */s*, *(es)*, or */es* at the end of a word to
       indicate the possibility of more than one item, and don't combine the
       singular and plural forms of a verb, such as *is/are*. Use the singular
       form or the plural form, use both forms joined by a conjunction, or use
       the phrase *one or more*.
     - *Use:*\

       Close any application that is open.

       Close any applications that are open.

       *Don't use:*

       Close any application(s) that is/are open.

Product names and version numbers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

When using Rackspace product names and showing version numbers, use
the following guidelines:

-  Always spell out and properly capitalize Rackspace product and
   service names (for example, Cloud Servers and Cloud Files).

-  In some cases, you can refer to the product generically after using
   the product name. For example, after you introduce the Cloud
   Monitoring Agent, you can refer to simply *the agent*.

-  Don't capitalize an item that a user creates through a Rackspace
   service. For example, users use the Cloud Servers service to create a
   *server*, not a *Server*, and they use the Cloud Load Balancer
   service to create a *load balancer*, not a *Load Balancer*.

-  Don't abbreviate Rackspace names, unless the abbreviation has been
   approved by the Legal and Marketing departments. For example, never
   abbreviate Cloud Block Storage as CBS.

-  For API documentation, the version number in the documentation should
   match the version number of the software. The combination of the API
   version number and the publication date identify the document
   version.

When using third-party company and product names, use the name as it's
used by the third-party. For a list of commonly used third-party names,
see :ref:`third-party-names-and-trademarks`.

When referring to an OpenStack service, use the actual service name, and
provide the project name in parentheses. For example, use OpenStack
Block Storage (Cinder). On subsequent references, use the service name
instead of the project name, unless you need to use project names to
differentiate between two versions of one service. See the `OpenStack
documentation
conventions <http://docs.openstack.org/contributor-guide/writing-style/openstack-components.html>`__
for service and project names.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - Use Cloud Servers to create a server.
     - Use Cloud Servers to create a Server.
   * - Use Cloud Block Storage to create volumes.
     - Use CBS to create volumes.
   * - You can add files to a server.
     - You can add Cloud Files to a Cloud Server.
   * - Microsoft SQL Server is supported.
     - MSSQL is supported.
   * - Cloud Servers provides the core features of the OpenStack Compute (Nova)
       API.
     - Cloud Servers provides the core features of OpenStack Nova.

.. _punctuation:

Punctuation
~~~~~~~~~~~

Use punctuation correctly and consistently. This section provides
guidelines for using punctuation in Rackspace documentation. For basic
rules about punctuation, see a grammar reference, such as the *Harbrace
College Handbook*.

-  `Ampersands <#ampersands>`__
-  `Colons <#colons>`__
-  `Commas <#commas>`__
-  `Dashes <#dashes>`__
-  `Ellipses <#ellipses>`__
-  `Exclamation points <#exclamation-points>`__
-  `Hyphens <#hyphens>`__
-  `Parentheses <#parentheses>`__
-  `Periods <#periods>`__
-  `Quotation marks <#quotation-marks>`__
-  `Semicolons <#semicolons>`__
-  `Slashes <#slashes>`__

Ampersands
----------

Don't use an ampersand (&) in text or headings to mean *and* unless you're
referring to the symbol on the UI. In the following example, the button name on
the UI includes an ampersand (&):

To continue, click **Save & Go to Step 3**.

Colons
------

Use the following guidelines for colons:

- Use a colon at the end of a sentence that introduces a list, table, figure,
  or example. If another sentence intervenes between the introduction and the
  thing being introduced, use a period instead of a colon.

- Use a colon at the end of the step to introduce substeps, a bullet list, or
  code that the user is expected to enter.

- In a list item, if you need to separate an initial term or phrase from the
  information that follows it, use a colon. For example:

  **Public**: This setting allows any two servers with public IP addresses to
  be load balanced. These can be nodes outside of the Rackspace network, but if
  they are, standard bandwidth rates apply.

- Don't use a colon at the end a table column header, a title, or a heading.

Commas
------

Use the following guidelines for commas. For basic comma usage, see a
grammar reference, such as the *Harbrace College Handbook*.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Guideline
     - Correct
     - Incorrect
   * - In a series of three or more items, use a serial comma (that is, precede
       the conjunction with a comma).
     - You can upgrade, migrate, and integrate the product.
     - You can upgrade, migrate and integrate the product.
   * - Don't use only a comma to separate independent clauses. Doing so
       creates a *comma splice*.

       If you join independent clauses, insert a coordinating conjunction (such
       as *and*) between them and precede the conjunction with a comma.
     - Click **Options**, and then click **Allow Fast Saves**.

       The UUID for ServiceNet is ``11111111-1111-1111-1111-111111111111``, and
       the UUID for PublicNet is ``00000000-0000-0000-0000-000000000000``.
     - Click **Options**, then click **Allow Fast Saves**.

       The UUID for ServiceNet is ``11111111-1111-1111-1111-111111111111``, the
       UUID for PublicNet is ``00000000-0000-0000-0000-000000000000``.
   * - Use a comma to set off a nonrestrictive clause (one that begins with
       *which*).

       Don't use a comma to set off a restrictive clause (one that begins with
       *that*).
     - The hourly backups are rolled into a nightly backup, which is retained
       for two days. *(nonrestrictive)*

       Enter the user name and password that you just created. *(restrictive)*
     - The hourly backups are rolled into a nightly backup which is retained
       for two days.

       Enter the user name and password, that you just created.
   * - Use a comma to separate an introductory word, phrase, or clause from the
       rest of the sentence.
     - When you check your email with an IMAP connection, you're accessing and
       managing your email directly from the email server.

       However, you can easily update the version by using the WordPress
       management dashboard.

       Unlike the other alarms in this list, you set the network check alarm
       variable upon network check creation.

       For more information, see Upgrading your Private Cloud.
     - When you check your email with an IMAP connection you're accessing and
       managing your email directly from the email server.

       However you can easily update the version by using the WordPress
       management dashboard.

       Unlike the other alarms in this list you set the network check alarm
       variable upon network check creation.

       For more information see Upgrading your Private Cloud.
   * - Don't use a comma between the verbs in a compound predicate.
     - These open-source Python clients run on Linux or Mac OS X systems and
       are easy to learn and use.
     - These open-source Python clients run on Linux or Mac OS X systems, and
       are easy to learn and use.
   * - When a comma is required after a quotation that's embedded in text,
       place the comma inside the closing quotation mark.
     - In the section called "Parameters," enter the values for length, width,
       and height.
     - In the section called "Parameters", enter the values for length, width,
       and height.
   * - Use commas in numbers with five or more digits. However, don't use
       commas in the following types of numbers: addresses, fractional parts of
       decimal numbers, page numbers, literal representations of user-entered
       values or displayed values

       **Note**: Don't use European-style numbering, which uses commas in the
       place of periods. For example, use 3.14159, not 3,14159.
     - 9001 N IH 35

       1452.7532

       page 1055

       1024 bytes
     - 9,001 N IH 35

       1,452.753,2

       page 1,055

       1,024 bytes
   * - When city and state names are embedded in a sentence, use a comma after
       the city and the state.
     - The company headquarters were in Kansas City, Missouri, before the
       merger.
     - The company headquarters were in Kansas City, Missouri before the
       merger.
   * - When a month, day, and year are embedded in a sentence, use a comma
       before and after the year. When only the month and year compose the
       date, omit the commas unless the syntax would ordinarily require a comma
       following the year.
     - The company acquired a German subsidiary on July 15, 2009, and is
       negotiating the purchase of a small Japanese company.

       The publications plan was printed in November 2010 in Austin.

       In December 2012, the database restoration failed.
     - The company acquired a German subsidiary on July 15, 2009 and is
       negotiating the purchase of a small Japanese company.

       The publications plan was printed in November, 2010, in Austin.

       In December 2012 the database restoration failed.

.. _dashes:

Dashes
------

An *em dash* is the longest dash. You can use em dashes to set off a long
qualifier in the middle of a sentence if the use of commas would hinder
readability. If you use em dashes for this purpose, don't use spaces around
them. (For an example, see the second paragraph in the following section,
"Ellipses.")

Don't use an em dash to separate a long sentence into two parts. Instead,
create two sentences.

An *en dash* is longer than a hyphen and shorter than an em dash. Most often,
you might use an en dash to show a range of numbers in a table or figure. For
example, 10–20 diagrams.

**Note:** To show a range of numbers in text, use *to* or *through* instead of
an en dash.

.. _ellipses:

Ellipses
--------

Use an ellipsis (...) in syntax or to indicate omitted code in code examples.

Don't use an ellipsis in header text of table columns or when showing the name
of an interface element—such as a text box, menu, menu command, or command
button—even if the ellipsis is displayed on the interface. For example, don't
use an ellipsis as follows:

- On the **File** menu, click **Open...**.
- Do this ... *(column header)*

Exclamation points
------------------

Avoid using exclamation points.

Hyphens
-------

This section provides general guidelines for hyphenation. For guidelines
about using dashes, see `Dashes <#dashes>`__.

-  `Hyphens in compound modifiers <#hyphens-in-compound-modifiers>`__
-  `Hyphens with prefixes <#hyphens-with-prefixes>`__

Hyphens in compound modifiers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

When two or more words precede and modify a noun as a unit (also called
a *compound modifier*), use hyphens according to the following
guidelines.

- To clarify meaning, use a hyphen. For example, *high-level-language compiler*
  is clearer than *high level language compiler.*

- Words that you hyphenate as compound modifiers preceding a noun might not be
  hyphenated in other parts of a sentence or when used as another part of
  speech. Hyphenate only if needed for clarity. For example,
  *local-level attributes* but *attributes defined at the local level*.

  **Note:** One exception is *up-to-date*, which is hyphenated in any position
  in a sentence.

- If the first component of a compound modifier is a number, use a hyphen. For
  example, *32-bit operating system*.

- If the first word of a compound modifier is an adverb ending in *-ly*, don't
  hyphenate the modifier. For example, *fully qualified domain name*.

- If one of the elements of a compound modifier is a trademark, don't hyphenate
  the modifier. For example, *Java specific*, not *Java-specific*.

Hyphens with prefixes
^^^^^^^^^^^^^^^^^^^^^

Words with prefixes aren't usually hyphenated. However, a hyphen might
be necessary in the following cases:

-  You need to distinguish between homographs, such as *re-create* and
   *recreate*.

-  The last letter of the prefix and the first letter of the root word
   are the same. Exceptions are words such as *reenter* and
   *preemptive*, which aren't likely to be misread.

-  The product team has hyphenated a term with a prefix, and you need to
   follow suit in the docs for consistency with the interface—for
   example, *multi-factor authentication* in the Identity product.
   Whenever possible, work with the teams to use preferred spelling.

For the correct formatting of a specific word, see a dictionary or
:ref:`alphabetical-list-of-terms`. For more information about
hyphenating prefixes, see *The Chicago Manual of Style*.

Parentheses
-----------

Avoid parentheses in running text. Parenthetical text can distract the
reader from the main idea of the sentence and disrupt the flow of the
sentence. When possible, put parenthetical information in a separate
sentence.

Following are some acceptable uses for parentheses:

-  To define an abbreviation
-  To show a special character
-  To show examples
-  To show a concise phrase that qualifies a term, title, or step

Don't add *(s)* or *(es)* to the end of a noun to indicate the
possibility of more than one item. Use the singular form or the plural
form, or use both forms joined by a conjunction.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - An access control list (ACL) allows access from an outside network into
       the ObjectRocket system.

       Object names can't contain characters such as dollar signs ($) and
       question marks (?).

       DNS is analogous to a phone book in that it assigns a numerical
       identifier (for example, 210.48.108.35) to a particular name (for
       example, www.diversity.net.nz).

       4. *(Optional)* Enter first and last name information for the mailbox
       owner.

       You can submit up to 10 messages (the default) in a single request.

Periods
-------

Use the following guidelines for periods. For basic period usage, see a
grammar reference, such as the *Harbrace College Handbook*.

- Use a period at the end of a declarative or imperative sentence, and insert
  only one space after the period.

- Place periods inside quotation marks, unless the quotation marks are part of
  a literal string. In such cases, place the period outside the quotation mark.

- Use periods in list items as follows:

  - If all of the items in a list are sentences, including imperative
    statements, end each item with a period.
  - If all of the items in a list are fragments, don't end the items with a
    period.
  - In a list of fragments, some or all of which are followed by sentences, end
    every fragment and sentence in the list with a period. For example, see
    the "Lists" topic.


- Use periods with abbreviations that could be misread as a word, such as *in.*
  (for *inch*). Also, use periods in the abbreviations *a.m.* and *p.m.*

- Precede a file name extension with a period.  Also, assume that the period in
  a file name extension is pronounced as *dot*, and use the indefinite article
  *a*. For example, a .**ini** file.

- Don't end a title or a heading with a period.

Quotation marks
---------------

Refer to quotation marks as *quotation marks*, not as *quote marks* or
*quotes*.

Use single and double quotation marks according to the following guidelines:

- Use quotation marks in user entries or syntax only if the software requires
  the quotation marks.

- Use quotation marks in message text only if the product shows quotation marks
  in the generated message. Use code font (monospace) to format messages.

- If you use a term in a unique or qualified sense, use double quotation marks
  in text only at its first occurrence, and omit the quotation marks in
  subsequent occurrences of the term. For example:

  The spelling checker "learns" the word. After it learns the word, the
  spelling checker ignores subsequent occurrences of the word in the document.

- Include appropriate punctuation, such as periods and commas, inside quotation
  marks unless the quotation marks are part of the syntax that the user must
  type.

- Don't use quotation marks for emphasis. Use italics instead, or other
  formatting as described in the "Text formatting" topic.

- Use quotation marks to enclose text that's used verbatim from another source,
  or to enclose quotations from people.

Semicolons
----------

Avoid using semicolons, which are often misused and, even when used
correctly, can make sentences longer and more difficult to understand.

- Instead of connecting independent clauses with a semicolon, break them into
  separate sentences.
- Instead of connecting more than two items with semicolons, create a list.

Slashes
-------

Don't use a slash mark (/) to present a choice among, or a series of,
actions or objects. Rewrite the phrase to eliminate the slash mark.
Exceptions are established terms like *client/server* and *read/write*.

Don't use a slash in dates. For information about how to format dates,
see :ref:`dates`.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Correct
     - Incorrect
   * - You can choose Cloud Backups, Cloud Files, or both.
     - You can choose Cloud Backups and/or Cloud Files.
       You can choose Cloud Backups/Files.
   * - To access your computer, plug it in, log in to the operating system, and
       type your password.
     - To access your computer, plug in the computer/log on/type your password.

Symbols
~~~~~~~

Symbols are used in code, as punctuation, with numbers, and to indicate
trademarks. Use the following general guidelines when you include
symbols in your documentation.

For guidelines about using specific marks of punctuation, see
`Punctuation <#punctuation>`__.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Guideline
     - Example
   * - When referring explicitly to a symbol in text, don't show only the
       symbol. Show the name of the symbol, or the name followed by the symbol
       in parentheses.

       On subsequent uses of the symbol, you can use just the name.

       If the symbol is a common mark of punctuation, like a period or a comma,
       don't show the mark in parentheses.
     - Escape the line by typing a backslash (/) character.

       To find files that were modified more than two days ago, type a plus
       sign (+) in front of the 2.

       Type a comma.
   * - Use a symbol *instead of* the name of the symbol only if space is
       limited (for example, in a table). Don't use symbols in running text.
     - *Body text:*

       45 percent

       16 degrees

       1,800 dollars

       *Limited space:*

       45%

       16º

       $1,800
   * - Don't insert a space between a number and a symbol, except when the
       symbol is used as a mathematical operator.
     - For files that use a total of 1,500 KB and a record size of 256, the
       equation is as follows: ``1,500,000 ÷ 256 = 5,860``
   * - To separate the options in a menu path, use right-angle brackets (>)
       surrounded by spaces.
     - Open Mac Mail and select **Preferences > Accounts**.

Tables
~~~~~~

Often text that's difficult to read in paragraph form is clear when put
into a table. Tables clarify the relationships among information, and
they're easy to scan. This topic provides the guidelines for the
following aspects of tables:

-  `Introductory text for tables <#introductory-text-for-tables>`__
-  `Table titles (captions) <#table-titles-captions>`__
-  `Column headers <#column-headers>`__
-  `Table text <#table-text>`__
-  `Table footnotes <#table-footnotes>`__
-  `Attribute or parameter tables in API
   documents <#attribute-or-parameter-tables-in-api-documents>`__

Table examples are presented in a separate section at the end of this
topic.

.. note::

   Don't create tables that are overly complex or that scroll
   horizontally. If you find that you have too much information in a table,
   try to break it up into smaller tables.

Introductory text for tables
----------------------------

In the text that precedes a table, introduce the table in a way that
relates the table to the text. If the table immediately follows the
reference to it, use a generic reference (such as *the following table*)
even if the table has a title. Provide a link to a table title only when
the table doesn't immediately follow the reference or when the table is
in a different article or section.

To introduce a table, use a sentence (not a fragment), and end it in a
period (not a colon).

Table titles (captions)
-----------------------

Tables should normally have titles (captions). However, some tables are
closely associated with the surrounding text and don't require titles.
For example, decision matrixes and tables within tasks, procedures, and
tutorials don't require numbers or titles.

When creating table titles, use the following guidelines:

- Use sentence-style capitalization for table titles. However, for
  words that are always uppercase or always lowercase, match that case.
- Don't start a table title with an article (*a*, *an*, *the*).
- Don't end a table title with a period or colon.
- Place the title above the table, not below it, and tag it as bold.
- Don't manually number table titles. If titles should be numbered, the style
  sheet will number them.
- Make table titles concise; limit them to one line if possible.
- Make table titles descriptive:

  - Avoid using a table title that duplicates a topic or section title.
  - Ensure that no two table titles in an article are identical. To distinguish
    between the titles that are similar, add qualifiers.

- Don't include trademark symbols in table titles.

Column headers
--------------

Use the following guidelines for text in column headers:

-  Use sentence-style capitalization in column headers. However, for
   words that are always uppercase or always lowercase, match that case.
-  Use singular nouns for column headers, unless the context requires
   otherwise.
-  Don't end column headers with ellipses or colons.

Table text
----------

Use the following guidelines for text in table cells:

-  Use the same punctuation and capitalization guidelines that you use
   for text in lists. See :ref:`writing-list-items`.
-  Make the entries in a table parallel. For example, in a column that
   describes options, be consistent in beginning the entries with a verb
   or noun.
-  Avoid leaving a table cell blank. If no information is available for
   that cell, use *Not applicable* or *None*. Use the abbreviation *NA*
   only if space constraints exist. Don't use dashes. An exception is
   for matrix-type tables that use an X or other marker to indicate
   support. In such cases, blank cells are acceptable (see the third
   example in the sidebar).
-  When showing a notation in a table, use the guidelines in `Notes and
   other notation types <#notes-and-other-notation-types>`__.
-  If space in a table is constrained, you can use abbreviations and
   symbols that you wouldn't normally use in body text (such as % for
   percent).
-  Don't use color to differentiate table text.

Table footnotes
---------------

If a notation (for example, a note or warning) applies to the entire
table, place the content in a regular notation preceding the table. If a
notation applies only to the content in a certain cell, place the
notation in that cell. However, if a notation applies to all of the
content in a row or column, or to the content in two or more cells, you
can use footnotes.

-  When writing the text of table footnotes, use the following
   guidelines:

   -  Ensure that all footnotes are written clearly and completely. Use
      sentences when possible. Avoid cryptic language.
   -  Ensure that all footnotes have parallel grammatical structure
      (sentences are paralleled by sentences, phrases by phrases, and so
      on).

-  Place the footnote text at the end of the table, either in a final
   row that spans the entire table or under the last row in the table.

-  Use superscript numbers to indicate the footnotes in the cells to
   which they apply. If numbers might be confusing (for example, because
   the text in the cells are numerical values), use lowercase letters
   instead.

   -  A footnote cited in a column header applies to the entire column.
   -  A footnote cited in a table cell applies to the text in that cell.
      Use a cell-level footnote if the note applies to multiple cells in
      the table.

Attribute or parameter tables in API documents
----------------------------------------------

When creating attribute or parameter tables in API documents, use the
following additional guidelines:

-  For tables that describes JSON or XML attributes, write the first
   sentence of a description with an implied subject. For example, if
   the attribute is name, the description might be as follows: "Server
   name, which becomes the initial host name of the server"
-  For attributes, include the valid values and default value at the end
   of the description. Use the formats "Valid values are *n* and *n*."
   and "The default is *n*." For example, "Valid values are ``true`` and
   ``false``." and "The default is ``false``."
-  If table descriptions or construction is complex, consider using a
   definition list or itemized list instead of a table.
-  Avoid putting definition lists in tables.

Examples
--------

The different parts of the preceding URL are explained in the following
table.

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Part of URL
     - Explanation
   * - ``swift://``
     - The prefix that passes file system requests to the Swift file system.
   * - ``acontainer``
     - The name of the container in Swift that contains the objects to be
       accessed. Container names must conform to RFC952 restrictions for host
       names—that is, the characters A-Z, numbers 0-9, and the hyphen (-).

       Nonconforming container names are inaccessible by swiftfs.
   * - ``aservice``
     - A user-friendly "service" name. A service name maps to a collection of
       configuration entries in the Hadoop core-site.xml file that specify
       where the container is located (for example, rackspace-dfw).
   * - ``/path/to/files``
     - The name of the object or objects in Swift to be referenced. Although
       Swift doesn't support paths, swiftfs attempts to interpret names that
       look like paths and behave appropriately. For example, an input path
       named ``/path/to/*`` would qualify all objects with names prefixed by
       ``/path/to/``. Similarly, an output path of ``/path/to/`` would prefix
       the names of all newly created objects with ``/path/to/``.

The following table provides the default values for the absolute limits.

**Absolute limits**

.. list-table::
   :widths: 25 50 25
   :header-rows: 1

   * - Name
     - Description
     - Limit (default value)
   * - Node count
     - Maximum number of allowed data nodes
     - 3
   * - Disk
     - Maximum disk capacity across all data nodes, in gigabytes (GB)
     - 4500
   * - RAM
     - Maximum RAM across all data nodes, in gigabytes (GB)
     - 23040
   * - VCPUs
     - Maximum virtual CPUs across all data nodes
     - 6

The following matrix indicates which upgrade scenarios are supported.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Upgrade scenario
     - Supported
     - Not supported
   * - 4.2.0 to 4.2.\ *x*
     -
     - X
   * - 4.1.\ *x* to 4.2.1
     - X
     -
   * - 4.1.\ *x* to 4.2.0
     -
     - X
   * - 4.1.\ *x* to 4.1.\ *x*
     - X
     -
   * - 4.0.0 to 4.2.\ *x*
     -
     - X
   * - 4.0.0 to 4.1.\ *x*
     - X
     -
   * - 3 (OpenCenter) to any version
     -
     - X
   * - 2 (Alamo) to any version
     -
     - X

The following chart compares these top content management systems
(CMSs).

.. list-table::
   :widths: 20 40 40
   :header-rows: 1

   * -
     - Drupal
     - WordPress
   * - **Homepage**
     - www.drupal.org
     - www.wordpress.org
   * - **About**
     - Drupal is a powerful, developer-friendly tool for building complex
       sites. Like most powerful tools, it requires some expertise and
       experience to operate.
     - WordPress began as an innovative, easy-to-use blogging platform. With an
       ever-increasing repertoire of themes, plug-ins, and widgets, this CMS is
       also widely used for other website formats.
   * - **Example sites**
     - Community Portal: Fast Company, Team Sugar
     - Social Networking: PlayStation Blog

       News Publishing: CNN Political Ticker

       Education/Research: NASA Ames Research Center

       News Publishing:The New York Observer
   * - **Installation**
     - Drupal Installation Forum
     - WordPress Installation Forum

.. _tasks:

Tasks
~~~~~

A *task* is an action that users perform to achieve a goal, such as creating a
server. A task topic, article, or section provides the action steps and the
necessary context and reference information that the user needs to complete the
task.

This topic provides guidelines for developing tasks.

-  `Task titles <#task-titles>`__
-  `Task introductions <#task-introductions>`__
-  `Prerequisites <#prerequisites>`__
-  `Procedures <#procedures>`__
-  `Steps <#steps>`__
-  `Results, verification, examples, and
   troubleshooting <#results-verification-examples-and-troubleshooting>`__
-  `Direction to the next action <#direction-to-the-next-action>`__
-  `Related topics <#related-topics>`__

Task titles
-----------

The title of a task topic, article, or section begins with the imperative form
of the task action, and it uniquely, precisely, and clearly describes the task.
Use a plural subject unless the singular makes more sense or is necessary for
clarity.

**Examples**

- Create users in SQL Server
- Configure SQL Server Management Studio to connect to SQL Server on Windows
- Add new ServiceNet routes to a server

For guidelines about capitalizing titles, see :ref:`capitalization`.

Task introductions
------------------

Before providing steps, set the context for the task as necessary. For example,
you could state the reason for completing the task, the method to be used, and
the expected result. You might also state the intended audience and suggest the
amount of time that the task might take, especially if it will take a long
time.

**Notes:**

- If the article or section title provides sufficient context, you
  can omit an introduction.
- Avoid providing extensive overview or conceptual text in the introduction to
  a task. Provide that information in a separate informational topic or in a
  topic that introduces the task as part of a larger process or user goal.

Prerequisites
-------------

If the task has requirements that the user *must* meet before taking action,
describe them in a "Prerequisites" section that precedes the steps. You could
include the following information:

-  A hyperlink to a preceding task, if that task must be performed
   before this task
-  Software that must already be installed, accessible, or running
-  Access rights that are required for users to perform the task
-  Hyperlinks to other topics that contain requirements or prerequisite
   tasks that the user must perform

.. note::

   Avoid including detailed procedures in a prerequisites section. Provide
   prerequisite tasks in other articles or sections, which you can reference in
   this section.

Procedures
----------

A task contains one or more *procedures*, or set of sequential action
steps. Consider the following guidelines when creating a procedure:

-  If the procedure has more than one step, use a numbered list for the
   steps. Don't use bullets, except to list choices within a step.
-  If the procedure has only one step, show that step in a regular
   paragraph. That is, don't number it.
-  If you have lengthy introductory or prerequisite information, or if
   you have more than one procedure, provide a heading for the procedure
   or procedures. Use the imperative form of the action and a singular
   form of the object. Don't repeat the title of the task article.
-  Try to limit procedures to 10 steps. If you have more than 10 steps,
   consider whether you can divide the steps into two or more
   procedures. Creating several short, simple, and sequential procedures
   instead on one long, complex procedure, especially one with many
   substeps and choice steps, will help users know where they are in
   the process, judge their progress, and complete the task
   successfully.

Steps
-----

When writing steps, use the following guidelines.

-  `Use imperative sentences <#use-imperative-sentences>`__
-  `Show one action per step <#show-one-action-per-step>`__
-  `Use consistent verbs <#use-consistent-verbs>`__
-  `Provide context before the
   action <#provide-context-before-the-action>`__
-  `Provide conditions before
   actions <#provide-conditions-before-actions>`__
-  `Follow the step with explanatory
   information <#follow-the-step-with-explanatory-information>`__
-  `Show only actions as steps <#show-only-actions-as-steps>`__
-  `Use screenshots sparingly <#use-screenshots-sparingly>`__
-  `Label optional steps <#label-optional-steps>`__
-  `Omit extraneous words <#omit-extraneous-words>`__
-  `Show multiple conditions in a
   list <#show-multiple-conditions-in-a-list>`__
-  `Show multiple possibilities in a
   list <#show-multiple-possibilities-in-a-list>`__
-  `Document only one method <#document-only-one-method>`__

Use imperative sentences
^^^^^^^^^^^^^^^^^^^^^^^^

Write each step as a complete and correctly punctuated imperative
sentence (that is, a sentence that starts with an imperative verb). In
steps, the focus is on the user, and the voice is active.

**Examples**

#. Log in to the Cloud Control Panel.

#. Use the following command to start ``vsftpd``:

   .. code::

      sudo service vsftpd start

Show one action per step
^^^^^^^^^^^^^^^^^^^^^^^^

Usually, include only a single action in each step. If two actions are
closely related, such as opening a menu and selecting a command from the
menu, you can include both actions in one step.

**Examples**

#. Under **Export**, select your database (for example, 388488\_drupal).

#. Scroll down to the bottom of the window and select the **Save as
   file** check box, which will save your database output to a file.

#. Click **Go**.

#. If you're prompted to save your file, save it to your computer.

Provide context before the action
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step specifies where to perform an action, state where to perform
the action before describing the action.

**Examples**

#. In the navigation pane, click **Inbound Rules**.


#. On the Binding and SSL Settings page, perform the following steps:

Provide conditions before actions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step specifies a situation or a condition, state the situation or
condition before describing the action.

**Examples**

#. If a new version is available, click **Install**.

#. To find out the encryption type of your Windows computer (32-bit or
   64-bit), navigate to the server's Control Panel and click **System**.

Follow the step with explanatory information
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Don't include explanatory or reference information in the action part
of a step. If needed, follow the step with one or more paragraphs that
provide supplemental information.

**Examples**

#. In the **Body Match** text box, enter a word or phrase that will
   appear on the page when it loads successfully.

   For example, you can perform a body match on the copyright date to
   verify whether the website is running.

Show only actions as steps
^^^^^^^^^^^^^^^^^^^^^^^^^^

Don't show system actions, responses, or results as steps. Put necessary
statements in unnumbered paragraphs following the steps to which they apply.
See the first example in the "Examples" section.

When the result of a step is the appearance of a dialog box, window, or page in
which the action of the next steps occurs, you can usually eliminate a result
statement and orient the user at the beginning of the next step. See the
second example in the "Examples" section.

**Examples**

*Use:*

#. On Linux, enter the following command:

   .. code::

      sudo rackspace-monitoring-agent --setup

   The list of setup settings is displayed.

*Use:*

#. Under **Other Options** in the Rackspace Email box, select **Mobile
   Sync**.
#. On the Activate Mobile Sync page, select individual users to
   activate, or select the **Add Mobile Sync to all mailboxes on this
   domain** option.

Use screenshots sparingly
^^^^^^^^^^^^^^^^^^^^^^^^^

Screenshots can help to orient the user, but a screenshot of every field or
dialog box usually isn't necessary.

If you include screenshots, place each one directly under the step that it
illustrates. Don't rely on the screenshot to show information or values that
the user must enter; always provide that information in the text of the steps.
However, ensure that the screenshot accurately reflects the directions and
values in the step text.

Label optional steps
^^^^^^^^^^^^^^^^^^^^

To indicate that a step is optional, include *(Optional)*, in italics,
as a qualifier at the beginning of the step.

**Example**

#. *(Optional)* Click **Advanced Options**.

Omit extraneous words
^^^^^^^^^^^^^^^^^^^^^

Omit extraneous words (such as *pop-up menu* or *command button*) unless
they're needed for clarity.

**Examples**

*Use:*

#. In the Disks window, right-click the volume and select **Take
   Offline**.

*Avoid:*

#. In the Disks window, right-click the volume and select **Take
   Offline** from the pop-up menu.

*Use:*

#. Click **Add**, enter a name for the profile, and then click **OK**.

*Avoid:*

#. Click the **Add** button, enter a name for the profile in the text
   box, and then click the **OK** button.

Show multiple possibilities in a list
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a step directs the user to choose from multiple possibilities,
use an unordered list to present the possibilities.

**Example**

#. Select a volume type:

   -  **Standard**: A standard SATA drive for users who need additional
      storage on their server
   -  **High Performance**: An SSD drive, which offers a higher performance
      option for databases and high performance applications

Document only one method
^^^^^^^^^^^^^^^^^^^^^^^^

If more than one method exists for completing an action, document only
one method, usually the most efficient or preferred method.

**Example**

*Use:*

#. Select **File > New**.

*Don't use:*

#. Select **File > New**, or press **Ctrl+N**.

Results, verification, examples, and troubleshooting
----------------------------------------------------

Following the procedure or procedures, include the following information
if it's necessary or helpful to the user. If the information is
brief, you can include it directly following the last step in the
procedure. If it's lengthy or you need to provide more than one type of
information, use sections with headings.

-  The result of performing the task.
-  Information about verifying successful completion of the task, such
   as the location of logs. If verification is a separate task in a
   different article or section, provide a hyperlink to it under a
   "Where to go from here" heading.
-  An example that illustrates or supports the task.
-  Information about what to do if the procedure doesn't work. This
   information might be a hyperlink to a separate troubleshooting topic.

Direction to the next action
----------------------------

If your task is part of a larger set of tasks, you can help the user
by including a "Where to go from here" section. You might include the
following information:

-  A brief explanation of the next task and why the user needs to
   perform it, accompanied by a hyperlink to the next task.
-  Hyperlinks to other tasks that could be done next, if multiple
   options are available. Describe the multiple options so that
   users know which task to choose.

Related topics
--------------

To provide a quick way for the user to access other content that's
related to the task, provide links to the content at the end of the
article or topic. Even if you have already included an embedded
hyperlink to the material in the article or topic, you can provide the
hyperlink again under "Related topics," but typically you should provide
a link only once in an article or section. For more information about
linking, see :ref:`links-and-cross-references`.

Telephone numbers
~~~~~~~~~~~~~~~~~

Use the following guidelines for telephone numbers:

Use a space, not hyphens or dashes, to separate parts of the telephone
number.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - 1 210 312 4600
     - 1-210-312-4600
   * - 1 800 961 4454
     - 1 (800) 961-4454

Precede US and Canadian telephone numbers with 1. Precede all other
telephone numbers with a plus sign.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - US and Canadian
     - All others
   * - 1 210 312 4600
     - +44 0 20 8734 2700

       +45 7734 5764

If you're showing phone numbers in screenshots or in examples, use the
following guidelines:

-  Don't use any number that might be a real telephone number. Instead,
   use a number in the range 555-0100 through 555-0199; these numbers
   are reserved for fictional use. You can also use a number that
   belongs to Rackspace.
-  If a screenshot includes a nonfictional, non Rackspace number, mask
   out all or parts of it.

.. _text-formatting:

Text formatting
~~~~~~~~~~~~~~~

Sometimes text should be formatted differently to designate a special meaning
or to make the text stand out. Usually this formatting is accomplished by
applying a different font treatment (bold, italics, or monospace).

.. note::

   *Monospace* is also called a *fixed-pitch* or *fixed-width*
   font. In monospace, each letter and character occupy the same amount of
   horizontal space. An example of a monospace font is Courier, and it
   looks as follows: ``monospace font``

Use the following general guidelines when formatting text:

-  To apply a font treatment, use the appropriate markup in your authoring
   tool. In RST, use a directive if one is available.
-  Don't apply font treatments to text in titles and headings.
-  Don't use capitalization to emphasize a term (for example, showing a
   general term in all capitals).
-  Don't use color alone to distinguish text.
-  Use quotation marks only as directed in this topic and in `Quotation
   marks <#quotation-marks>`__.

The following table shows the text formatting to use for different text
elements. The following style differences are highlighted:

- Content for Public Cloud versus Private Cloud
- Content that documents a CLI or API versus a GUI

.. list-table::
   :widths: 30 20 50
   :header-rows: 1

   * - Text element
     - Treatment
     - Output example
   * - API operation names
     - Regular text

       All lowercase
     - The following table describes the request attributes for the operation
       for migrating vaults.
   * - Application names
     - Regular text
     - You must configure the RabbitMQ application.
   * - Area (group box) names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - Argument names
     - Monospace
     - To list or retrieve files from a node that's running the OpenCenter
       agent, use the ``file`` argument with the ``opencentercli`` node
       command.
   * - Attribute names
     - Monospace
     - The ``expires`` attribute denotes the time after which the token
       automatically becomes invalid.
   * - Box names
       (check box, combo box, group box, list box, spin box, text box, but not
       dialog box)
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select the **Manually configure server settings or additional server
       types** check box.

       Retype the password that you entered in the **Password** box.
   * - Button names
       (command, option, radio)
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Cascades
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Check box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select the **Manually configure server settings or additional server
       types** check box.
   * - Code
     - Monospace

       In RST, apply the ``.. code-block:: console`` directive.
     - ``$ grep "ftp" /etc/xinetd.d/*`` ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``

       To set the environment variable, run ``export token="token"``.
   * - Column names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - You can sort the backups by server by clicking the **Server** column
       label.
   * - Combo box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select a name from the **Send to** list, or type a new name.
   * - Command names (CLI)
     - *(Public)* Monospace

       *(Private)* Bold, by applying the ``:command:`` directive in RST
     - *(Public)* You can check the architecture on Linux by using the ``uname
       -a`` command.

       *(Private)* You can check the architecture on Linux by using the **uname
       -a** command.
   * - Command syntax
     - Monospace
     - If a service isn't running, use the service command to start it, as
       follows:

       ``$ sudo service httpd start``
   * - Cross-references
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - Database names
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* Start by creating a new database called **mytestdb**.

       *(CLI)* Start by creating a new database called ``mytestdb``.
   * - Dialog box names
     - Regular text
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.
   * - Directory names
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* Place all the contents of the uncompressed **wordpress**
       directory (excluding the directory itself) into the **/web/content/**
       directory, which is the root directory of the site.

       *(Private)* Place all the contents of the uncompressed ``wordpress``
       directory (excluding the directory itself) into the ``/web/content/``
       directory, which is the root directory of the site.

       *(CLI)* The following example shows a basic configuration for the FTP
       service, in a file in the ``/etc/xinetd.d directory``.
   * - Document titles
     - Italic

       **Note**: Use italic even if the title is a hyperlink.

     - For the most up-to-date information about rate and absolute limits, see
       the "Limits" section in the *Rackspace Cloud Databases Developer Guide*.
   * - Element names
     - Monospace
     - The ``message`` element returns a human-readable message that's
       appropriate for display to the end user.
   * - Email addresses
     - For examples, use bold.

       For actual email address, use the convention in your authoring
       environment to make the email address live.
     - **yourName@example.com**

       Contact the editor at kelly.holcomb@rackspace.com.
   * - Emphasis
     - Italic
     - Offset *must* be a multiple of the limit (or zero); otherwise, a Bad
       Request exception is generated.
   * - Environment variables
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.
   * - Error messages
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       .. code::

          The user doesn't have permission to perform this action.

   * - Examples, code
     - Monospace
     - ``$ grep "ftp" /etc/xinetd.d/*`` ``/etc/xinetd.d/vsftpd:service ftp``
       ``/etc/xinetd.d/vsftpd:server = /usr/sbin/vsftpd``
   * - Field names, GUI
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Database Name** field, enter a database name identifier.
   * - File names and extensions
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* To remove the **vs\_quantum-api.cfg** file from the
       **haproxy.d** directory and retain it, you can move it to another
       directory.

       *(Private, CLI)* To remove the ``vs_quantum-api.cfg`` file from the
       ``haproxy.d`` directory and retain it, you can move it to another
       directory.
   * - Flags
     - Monospace
     - Use the ``-t`` flag to add a time stamp to the results.
   * - Folder names
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* Copy the **index.php** file from your computer to the
       **content** folder.

       *(CLI)* Copy the ``index.php`` file from your computer to the
       ``content`` folder.
   * - Functions
     - Monospace
     - Container names are sorted based on a binary comparison, a single
       built-in collating sequence that compares string data using the
       ``memcmp()`` function, regardless of text encoding.
   * - Glossary terms
     - Italic, by applying the ``:term:`` directive in RST

       This directive also links the term to the definition in the glossary.
     - Rackspace provides an *IaaS* solution through a variety of complementary
       *services*.
   * - Group box names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the **Edit Signature** area, enter the text that you want to appear
       in your signature.
   * - GUI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - HTML tags
     - Monospace
     - Avoid putting the ``xml:id`` attribute on the ``title`` tag.
   * - Hyperlinks (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - Icon names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - To verify which OS version you're running, click the **Apple** icon in
       the top-left corner and then select **About This Mac**.
   * - Keyboard key combinations, names, and shortcuts
     - *(Public)* Bold

       *(Private)* Monospace
     - *(Public)* Press **Shift-G** and then press **Enter**.

       *(Private)* Press ``Shift-G`` and then press ``Enter``.
   * - Letters as letters
     - Italic
     - Place *i* before *e* except after *c*.
   * - Links (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - List box names and selections
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - From the **Account Type** list, select **Exchange 2007**.

       To view these settings, select **Configure Backup** from the **Backup
       Actions** list.
   * - Menu names, commands, and sequences
     - Bold

       In RST, apply the ``:menuselection:`` directive to sequences.
     - Right-click the volume and select **Take Offline**.

       From the **Outlook** menu, select **Preferences**.

       Select **Start > Control Panel**, and then click the **Mail** icon.
   * - Messages (error, warning)
     - Monospace
     - In SQL Server Management Studio, when you right-click a SQL Server 2012
       database and selecting **Properties**, the following error message
       appears:

       .. code::

          The user doesn't have permission to perform this action.

   * - Method names (HTTP)
     - Bold

       All capitals
     - Client authentication is provided through a REST interface by using the
       **GET** method.
   * - New terms
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Option names, command
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``--ip-addresses`` option specifies the IP address and an alias for
       the target.
   * - Option button names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Package names
     - Monospace
     - You must install the ``libvirt`` package.
   * - Page names
     - Regular text
     - On the Preferences page, you determine how frequently you receive email
       about all the activity on your account: daily, weekly, or both.

       On the Server Settings page, click **Check Name**, type your password,
       and then click **OK**.
   * - Panes, named and unnamed
     - Regular text
     - To verify that your SSL binding works, select your website in the
       Connections pane (if it's not already selected) and then click **Browse
       *ipAddress* (https)** in the Actions pane.

       In the navigation pane, select **Composing Email**.
   * - Parameter names
     - Monospace

       In RST, apply the ``:option:`` directive.
     - The ``display_description`` parameter is optional.

       Use the ``--flavor`` and ``--image`` parameters to specify the IDs or
       names of the flavor and image to use for the image.
   * - Paths
     - *(Public, GUI)* Bold

       *(Private, CLI)* Monospace
     - *(Public, GUI)* The path to Perl is **#!/usr/bin/perl -w**.

       *(Public, GUI)* In the URI path
       **https://incident.api.rackspacecloud.com/v1/...**, the API version is
       1.

       *(Private, CLI)* The path to Perl is ``#!/usr/bin/perl -w``.

       *(Private, CLI)* In the URI path
       ``https://incident.api.rackspacecloud.com/v1/...``, the API version is
       1.
   * - Permissions
     - Regular text
     - Log in to a shell as the user who has write permissions to
       ``/usr/local/bin`` on your local computer.
   * - Placeholder (variable) text
     - See `Placeholder (variable) text <#placeholder-variable-text>`__
     - Not applicable
   * - Privileges
     - Regular text
     - The following examples assume that you're making the firewall changes
       as a normal user with sudo privileges.

       The user is granted ALL privileges on the database.
   * - Qualifiers
     - Italic
     - 1. *(Optional)* Enter a new name for the image.

       You can tell that the Managed Cloud post-build automation has
       successfully completed as follows:

       *(Windows servers)* The following file is created:
       **C:\\windows\\temp\\rs\_managed\_cloud\_automation\_complete.txt**

       *(Linux servers)* The following file is created:
       **/tmp/rs\_managed\_cloud\_automation\_complete**
   * - Quotations

       (content quoted from another source)
     - Quotation marks, or block quote formatting
     - "Scalability is key for our business," explained Nathan Goff, Inavero
       Operations Director and Partner. "There's nothing worse than making our
       clients look bad to their customers."
   * - Radio button names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - Select **Microsoft Exchange** and then click **Next**.
   * - Role names
     - Regular text
     - The full access role has the permissions to create, read, update, and
       delete resources within multiple designated products where access is
       granted.
   * - Sequences
       (menu, field)
     - Bold

       Use **>** to separate.

       In RST, apply the ``:menuselection:`` directive.
     - Select **Start > Control Panel**, and then click the **Mail** icon.

       You can find more documentation about RackConnect in the **Community >
       Discussions > RackConnect** section of the MyRackspace Portal.
   * - Syntax statements
     - Monospace
     - The main command used to change a file’s owner or group is ``chown``.
       The most common syntax used with ``chown`` is as follows:

       ``chown user:group file1 file2 file3``
   * - Tab names
     - Bold

       In RST, apply the ``:guilabel:`` directive.
     - In the Microsoft Exchange dialog box, click the **Connection** tab and
       then select the **Connect to Microsoft Exchange using HTTP** check box.
   * - Terms, new
     - Italic
     - Cloud Servers that are built using the base Linux images are created
       without a dedicated swap partition and with *swappiness* (a measure of
       how the Linux kernel tries to use swap memory) set to 0.
   * - Terms, unique sense
     - Regular text

       Quotation marks on first use
     - The spelling checker "learns" the word. After it learns the word, the
       spelling checker ignores subsequent occurrences of the word in the
       document.
   * - UI labels
     - Bold

       In RST, apply the ``:guilabel:`` directive.

       **Exception:** Show window, dialog box, wizard, page, panel, and screen
       names in regular text unless they need to be distinguished from the
       surrounding text. In such cases, use bold.
     - In the Microsoft Exchange dialog box, click **Apply** and then click
       **OK**.

       On the Choose Service page, select **Microsoft Exchange or compatible
       service**, and then click **Next**.

       Read the preliminary steps in the Configure Your Server wizard, and then
       click **Next**.
   * - URLs (not live)
     - Bold
     - To access the web interface, open your web browser and navigate to
       **http://yourDomain.com/zipit-install.php**.
   * - URLs (live)
     - See :ref:`links-and-cross-references`.
     - Not applicable
   * - User input
     - *(GUI)* Bold

       *(CLI)* Monospace
     - *(GUI)* In the **Server** text box, type **outlook**.

       *(CLI)* Create a file by using a text editor, and insert the following
       code: ``<?php phpinfo(); ?>``

       *(CLI)* For the username, enter ``admin``.
   * - Variable (placeholder) text
     - See `Placeholder (variable) text <#placeholder-variable-text>`__
     - Not applicable
   * - Variables, environment
     - Monospace
     - You can set the ``MYSQL_HOST`` environment variable to the remote host's
       address.

       You can export the tenant ID to the ``$account`` environment variable
       and the authentication token to the ``$token`` environment variable.
   * - Window names
     - Regular text
     - In the Network Connections window, right-click the private adapter and
       select **Properties**.
   * - Wizard names and wizard page names
     - Regular text
     - On the Welcome page of the Active Directory Domain Services Installation
       Wizard, ensure that the **Use advanced mode installation** check box is
       cleared, and then click **Next**.
   * - Words as words
     - Italic
     - Don't use *button* and *icon* interchangeably. If you're referring to
       a command button or toolbar button (labeled or unlabeled), use *button*.
       If you're referring to a graphic on a screen, window, or other area,
       use *icon*.

Time
~~~~

You can show time by using either the 12-hour or 24-hour clock. The
preferred format for international audiences, and the format used in
most computer systems, is the 24-hour clock. Use the 24-hour clock when
possible. If the technology or interface that you're documenting shows
or uses the 12-hour clock, then be consistent with the interface.

24-hour clock
-------------

When you use the 24-hour clock to show time, use the following
guidelines:

-  Separate the hours, minutes, and seconds by using a colon.
-  Show the hours, minutes, and second with two digits each, even if the
   leading digit is 0.
-  If you need to show a time zone, use Coordinated Universal Time
   (UTC), and indicate the time-zone offset from UTC.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - 08:29:37
   * - 18:30:59
   * - 18:00:00 to 20:30:00
   * - 10:30:00 (UTC -6) (refers to CT)
   * - 12:00:00 (noon)
   * - 00:00:00 (midnight)

12-hour clock
-------------

When you use the 12-hour clock to show time, use the following
guidelines:

-  Separate the hours and minutes by using a colon. If the minutes are
   00, you don't need to show them unless you're showing a span of
   time that includes a time with minutes.
-  Use lowercase letters for abbreviations of ante meridiem (a.m.) and
   post meridiem (p.m.). Separate these abbreviation from the time with
   a space. Use periods in the abbreviations.
-  When specifying time zones, show both the spelled-out name and the
   abbreviation. Show the name in lowercase letters; use uppercase
   letters and no periods for the abbreviation.
-  Avoid references to standard and daylight saving time because the
   appropriate designation changes frequently. However, if you need to
   include such a reference, insert *S* (for standard) or *D* (for
   daylight) as the second character in the abbreviation.
-  When referring to 12 a.m., use *12 midnight* or just *midnight*. When
   referring to 12 p.m., use *12 noon* or just *noon*.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Examples
   * - 10:29 a.m.
   * - 6 p.m.
   * - 6:00 p.m. to 8:30 p.m.
   * - 10:30 a.m. central time (CT)
   * - 1:30 p.m. central standard time (CST)
   * - midnight

.. _titles-and-headings:

Titles and headings
~~~~~~~~~~~~~~~~~~~

This topic provides guidelines for creating titles and headings in
documentation.

-  `Capitalization <#capitalization>`__
-  `Style and structure <#style-and-structure>`__
-  `Text following titles and
   headings <#text-following-titles-and-headings>`__
-  `Tables of contents <#tables-of-contents>`__

Capitalization
--------------

Use *sentence-style* capitalization for most titles and headings,
including article, chapter, table, figure, and example titles, as well
as section and procedure headings.

One exception is guide titles, which use *title-style* capitalization.

For capitalization guidelines, see :ref:`sentence-style-capitalization` and
:ref:`title-style-capitalization`.

Style and structure
-------------------

Use the guidelines in this section to create effective and consistent titles
and headings. The following guidelines apply to all titles and headings;
special considerations for stand-alone articles, product guides, and tables,
figures, and examples follow this list.

- Create succinct, meaningful, descriptive titles and headings, and place the
  most important words first.

- Ensure that each title and heading is unique within a given content set.

- Include articles, prepositions, and punctuation as needed for clarity.
  However, avoid using an article (*a*, *an*, or *the*) as the first word.

- Avoid showing both an abbreviation and its spelled-out term in a title or
  heading. To help control the length of titles and headings, show the
  abbreviation in the title or heading and then define it in the first
  paragraph of the text.

- If you show a literal term (such as a command or option name) in a title or
  heading, follow it with an appropriate noun.

- Don't end a title or heading with a colon or period. If the title or heading
  is in the form of a question, end it with a question mark.

- Don't apply font treatments (bold, italics, or monospace) to text in a title
  or heading.

- Don't include trademark symbols in titles or headings. Show the symbol on the
  first use of the trademark in text.

- Avoid having only a single heading at any level (for example, a single
  subsection in an article or section). If you find that you have a single
  heading at any one level, consider whether you can reorganize the information
  to either eliminate the heading or add a second one at that level.

- Avoid having more than two levels of sections within an article or topic. If
  you use more than two levels of sections, consider whether you can reorganize
  to make the structure flatter.

- Don’t "stack" titles or headings. That is, don’t immediately follow a title
  or heading with another title or heading. Text should always intervene
  between them. Ensure that such text is meaningful. If it is just filler text,
  consider whether you can restructure the content.

- Use a consistent grammatical structure for the titles and headings of
  specific types of content:

  .. list-table::
     :widths: 15 25 30 30
     :header-rows: 1

     * - Type
       - Grammatical structure
       - Stand-alone article examples
       - Product guide examples
     * - Conceptual
       - Any grammatical structure that's appropriate, except a verb, gerund, or
         infinitive
       - Linux distributions

         Best practices for backing up your data
       - Core concepts

         How monitoring works

         Limitations of detaching from Rackspace networks
     * - Step-by-step instructions (a task)
       - An imperative verb

         **Note**: For specific guidelines for headings within tasks, see
         :ref:`tasks`.
       - Identify network interfaces on Linux

         Prepare data disks on servers running Windows

         Set up Mobile Sync for Webmail
       - Sign up for a Rackspace Cloud account

         Authenticate with the nova client
     * - Tutorial or high-level process
       - A gerund
       - Understanding logrotate

         Customizing Apache web logs
       - Working with your first message queue
     * - Reference
       - A plural noun or a noun phrase
       - Permissions matrix for Cloud Networks

         Rackspace Auto Scale glossary
       - Environment variables for the nova and supernova clients

         Restore operations

         cURL command summary
     * - Troubleshooting
       - A grammatical structure that's appropriate for the type of content (a
         troubleshooting topic can contain task, tutorial, concept, or reference
         information)
       - Troubleshoot alarms

         Service troubleshooting on Linux
       - Troubleshooting
     * - FAQ
       - A descriptive noun or noun phrase, followed by *FAQ*
       - Rackspace Cloud Billing FAQ

         Scheduled images FAQ
       - Not applicable

Stand-alone articles
^^^^^^^^^^^^^^^^^^^^

In addition to the preceding guidelines, use the following guidelines when
creating titles and headings for stand-alone articles on the Support site or in
other collections of documentation:

- Create article titles that don’t rely on body text or other titles for their
  meaning (that are, in other words, independent of context). Users should be
  able to tell from a title whether the information in the article is relevant
  to their needs. Avoid ambiguous one-word titles, such as "Overview."

- Don't number titles to indicate their placement in a series of articles.
  Indicate the order of articles within the content of the article, referring
  users to information that they should have read previously before reading the
  current article. Use links to provide navigation to preceding and following
  articles in the series.

- Start with the highest level of heading that is approved for headings
  (for example, h3), and do not skip heading levels.

Product guides
^^^^^^^^^^^^^^

In addition to the preceding guidelines, use the following guidelines when
creating titles and headings for sections in product guides:

- If possible, limit titles and headings to 60 characters for legibility in the
  TOC pane.

- Consider that titles and headings are written within the context of the
  content set in which they are presented. Therefore, you can usually omit
  "context-setting" terms. For example, if the content set is about servers,
  you can usually omit "for servers" from the title or heading.
  (For example, "Attach a network to a server" can be shortened to
  "Attach a network" with no loss of clarity.)

- Define consistent heading levels, and do not skip levels.

Tables, figures, and examples
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

As a general rule, tables, figures, and examples should have titles
(also called captions). However, tables, figures, and examples in
procedures and tutorials don't normally require titles.

In addition to the preceding guidelines, use the following guidelines when
creating titles for tables, figures, and examples:

-  Place the title above the table, figure, or example, not below it.

-  Avoid using a title that duplicates an article or section title.

Text following titles and headings
----------------------------------

Don’t immediately follow a title or heading with another title or heading.
Instead, follow a title or heading with body text.

The body text must be independent from the title or heading. Don't use a title
or heading as an antecedent in the sentence that follows it. That is, be sure
to repeat the subject in the first sentence that follows the title or heading,
rather than using a pronoun that refers to the title or heading as its
antecedent.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Don't use
   * - **Identify network interfaces on Linux**

       This article briefly describes how to identify which network interfaces
       on a Linux server are associated with which IP addresses.
     - **Identify network interfaces on Linux**

       This article briefly describes how to do this.

Tables of contents
------------------

In addition to using the preceding guidelines when creating titles and
headings, use the following guidelines when creating a table of
contents (TOC) for a collection of content:

-  Entries in the TOC should link only to sections in the content. Don't
   include a link to an outside resource in the TOC.

-  The text of a TOC entry must match the text of the title or heading
   to which it links. If the link needs to be shorter, revise the
   title or heading to be shorter.

-  Don't manually format the TOC. TOC formatting must be consistent and
   controlled by the code.

.. _trademarks:

Trademarks
~~~~~~~~~~

Using Rackspace trademarks correctly protects Rackspace brands and
intellectual property, and promotes our reputation. Using third-party
trademarks correctly protects Rackspace from legal action.

Rackspace Legal has created comprehensive guidelines for using
trademarks at Rackspace. To get a comprehensive view of trademarks, read
the `21-page
PDF <https://one.rackspace.com/pages/worddav/preview.action?fileName=RACKSPACE-%2327629-v1-Rackspace_Trademark_Guidelines.pdf&pageId=72684499>`__.
If you're interested in only what you need to know to comply with
guidelines in your documentation, review the guidelines in this topic.

Examples of trademarks
----------------------

Following are examples of Rackspace trademarks:

-  Fanatical Support
-  Rackspace (when used in connection with service names)
-  Rackspace Managed Hosting
-  RackConnect

For a complete list, see the `Rackspace Trademark
List <https://www.rackspace.com/information/legal/tmlist>`__.

Following are examples of third-party trademarks that are often used in
our content:

- Apache
- Enterprise Linux
- Linux
- OpenStack
- Python
- Red Hat
- SQL Server
- Ubuntu

If you need to verify whether a name is a trademark, see that company's
website.

Trademark usage guidelines
--------------------------

Use the following guidelines when showing Rackspace and third-party
trademarks in documentation.

.. list-table::
   :widths: 40 30 30
   :header-rows: 1

   * - Guideline
     - Example — Use
     - Example — Don't use
   * - Show a trademark exactly as it's shown by the owning company (Rackspace
       or third-party). Don't change the capitalization or abbreviate the
       trademark.

       Abbreviations are acceptable only if they're used by the owning company
       and also trademarked.
     - This article describes the process of backing up a Microsoft SQL Server
       2008 database. These actions need to be completed by the Administrator
       user or by a user who is part of the SQL Server Admin user group.
     - This article describes the process of backing up an MS SQL Server 2008
       database. These actions need to be completed by the Administrator user
       or by a user that's part of the MS SQL Admin user group.
   * - Use trademarks as adjectives on first use in the text of an article or
       chapter, and as often as possible after that.

       After first use, you can use the trademark as an noun if it's clear
       that you're referring to that trademark.

       Don't use a trademark as a verb.
     - Each cloud server has a single private IP address. When you use the
       RackConnect solution, if you need direct access to the cloud server from
       the Internet, you can use the public IP assigned to the server in
       RackConnect.
     - Each cloud server has a single private IP address. When you use the
       RackConnect, if you need direct access to the cloud server from the
       Internet, you can use the public IP assigned to the RackConnected cloud
       server.
   * - Don't combine a trademark with any other term, including another
       trademark. For example, don't attach a trademark to another term by
       using a hyphen or slash.
     - On Linux, Mac OS X, and other operating systems based on UNIX, you
       usually use the ssh command to connect to a server via SSH.
     - On Linux, Mac OS X, and other UNIX-based operating systems. you usually
       use the ssh command to connect to a server via SSH.
   * - Don't use a trademark as a possessive or as a plural. If necessary,
       form a possessive or plural from the noun that follows the trademark
       (which is used as an adjective).
     - The packaged version of NGINX from Ubuntu uses a sites-available and
       sites-enabled layout in the same manner as an Apache installation based
       on Debian.
     - Ubuntu's packaged version of NGINX uses a sites-available and
       sites-enabled layout in the same manner as a Debian-based Apache
       installation.
   * - Always distinguish a third-party trademark from a Rackspace product name
       or trademark. Generally you can do this through ensuring that words
       intervene between the trademarks.

       Show trademarks of different companies together only if a license or
       agreement exists between the two companies. In such cases, use italics
       to distinguish one trademark from the other. You can generally do this
       just on first use of the two terms together in the document or article.
     - The version of MySQL installed on Cloud Sites that use Windows
       technology is currently MySQL Connector version 5.2.5.

       The Rackspace Cloud Storage App for Microsoft SharePoint enables you to
       work with files inside of Rackspace Cloud Files alongside SharePoint
       content.
     - The version of MySQL installed on Windows Cloud Sites is currently MySQL
       Connector version 5.2.5.

       The Rackspace Cloud Storage App for Microsoft SharePoint enables you to
       work with files inside of Rackspace Cloud Files alongside SharePoint
       content.
   * - Always use *Fanatical Support* as a trademark. Don't use *fanatical*
       outside of the trademark. Also, always distinguish this trademark from
       surrounding text by using bold and italics (in RST, apply the
       ``:bolditalic:`` directive). Show a registered trademark symbol on first
       use.

       For more information, see the `Rackspace Trademark Guidelines PDF from
       Legal
       <https://one.rackspace.com/pages/worddav/preview.action?fileName=RACKSPACE-%2327629-v1-Rackspace_Trademark_Guidelines.pdf&pageId=72684499>`__.
     - We provide :bolditalic:`Fanatical Support` ®.
     - Our support is fanatical.

URLs and domain names
~~~~~~~~~~~~~~~~~~~~~

Some samples, such as those related to the Customer Service Layer API,
include a sample customer's URL or email address. Don't invent a fake
domain name for this purpose. Even if that name isn't registered today,
someone might claim it tomorrow. Instead, use a domain name permanently
reserved for the purpose of demonstration and documentation.
**example.com** and **example.org** are reserved globally by the
Internet Assigned Numbers Authority (IANA).

Because the domain named **example.com** and the user named *Joe User*
don't and never will exist, it's safe to use the email address
**joe.user@example.com**.
