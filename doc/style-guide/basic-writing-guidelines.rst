.. _writing-guidelines:

========================
Writing guidelines
========================

Use these writing guidelines to create Rackspace content that's clear and
consistent, and that helps users accomplish their goals.

Use active voice
~~~~~~~~~~~~~~~~

Active voice makes the performer of the action, usually the user, the subject
of the sentence. Sentences that use the active voice are usually easier to
understand than sentences that use the passive voice.

In passive voice, the recipient (not the performer) of the action is the
subject of the sentence. Passive voice is usually less engaging and more
complicated than active voice. When you use passive voice, the actions and
responses of the technology can be difficult to distinguish from those of the
user. In addition, passive voice usually requires more words than active voice.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - After you install the software, start the computer.
     - After the software has been installed, the computer can be started.
   * - Click **OK** to save the configuration.
     - The configuration is saved when the **OK** button is clicked.
   * - Create a server.
     - A server is created by you.
   * - Rackspace products and services solve your business problems.
     - Your business problems are solved by Rackspace products and services.

Passive voice is acceptable in the following situations:

-  Using active voice sounds like you're blaming the user. For
   example, you can use passive voice in an error message or
   troubleshooting content when the active subject is the user.
-  The performer of action is unknown, or you want to de-emphasize the
   performer of the action and emphasize the object on which the action is
   performed.
-  Using active voice makes the sentence wordy or awkward.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Acceptable (passive)
     - Avoid (active)
     - Why?
   * - If the build fails, the flavor might have been omitted.
     - If the build fails, you probably omitted the flavor.
     - The active voice blames the user.
   * - A flag was set incorrectly.
     - You set the flag incorrectly.
     - The active voice blames the user.
   * - Account owners can't be assigned additional roles, and their access
       can't be restricted.
     - Administrators can't assign account owners additional roles, and they
       can't restrict the access of account owners.
     - In this context, the object, account owners, is more important than the
       actor, administrators.

Use present tense
~~~~~~~~~~~~~~~~~

Users read documentation to perform tasks or gather information. For them,
these activities occur in their present, so the present tense is appropriate in
most content. Additionally, present tense is easier to read than past or future
tense.

Use future tense only when you need to emphasize that something will occur
later, from the users' perspective.

.. tip::

   To easily find and remove instances of future tense, search for *will*.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - The product **prompts** you to verify the deletion.
     - The product **will prompt** you to verify the deletion.
   * - After you log in, your account **begins** the verification process.
     - After you log in, your account **will then begin** the verification
       process.
   * - To back up Cloud Sites to Cloud Files by using this example, you
       **create** two cron jobs. One job **backs up** the cloud site and
       database, and the second job **uploads** the backup to Cloud Files.
     - To back up Cloud Sites to Cloud Files by using this example, you **will
       need to create** two cron jobs. One cron job **will back up** the cloud
       site and database, and the second cron job **will upload** the backup to
       Cloud Files.
   * - Any customer with a Cloud account **can provision** multiple ServiceNet
       database instances.
     - Any customer with a Cloud account **will be able to provision** multiple
       ServiceNet database instances.
   * - When the contract changes, Rackspace **will notify** customers in
       release notes.
     - Not applicable. Future tense is appropriate in this example.

.. _write-to-the-user:

Write to the user by using second person and imperative mood
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Users are more engaged with documentation when it talks to them directly. You
accomplish this by using second person, that is, addressing the user as *you*.
Second person also promotes a friendly tone.

-  Use second person with the imperative mood (in which the subject *you* is
   understood) and active voice to eliminate wordiness and confusion about who
   or what initiates an action, especially in procedural steps.

-  Use second person to avoid the use of gender-specific, third-person pronouns
   such as *he*, *she*, *his*, and *hers*. If you must use third person, use
   the pronouns *they* and *their*, but ensure that the noun that the pronoun
   refers to is plural.

-  Use first-person plural pronouns (*we*, *our*) judiciously. These pronouns
   emphasize the writer or Rackspace rather than the user, so before you us
   them, consider whether second person or imperative mood is more "user
   friendly." However, use *we recommend* rather than *it's recommended* or
   *Rackspace recommends*. Also, you can use *we* in the place of *Rackspace*
   if necessary.

-  Use the first-person singular pronoun *I* only in the question part of FAQs
   and when authors of blogs or signed articles are describing their own
   actions or opinions.

-  Avoid switching person (point of view) in the same document. Switching
   person is acceptable, however, in blog posts that use first-person singular
   but then switch to second person for instructional steps.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - To create a server, you specify a name, flavor, and image.
     - To create a server, specify a name, flavor, and image. (imperative mood)
   * - Creating a server involves specifying a name, flavor, and image.
     - To create a server, the user specifies and name, flavor, and image.
   * - Click **Yes** to accept the license agreement.
     - The license agreement is accepted when the user clicks **Yes**.
   * - We offer you a comprehensive portfolio of hosting options.
     - Rackspace offers a comprehensive portfolio of hosting options for the
       enterprise buyer.
   * - Fanatical Support sets Rackspace apart. We are here to help, 24x7x365.
     - Rackspace is here to help customers.
   * - Cloud Backup uses block-level deduplication, which means that only those
       parts of a file that have changed are saved.
     - Cloud Backup uses block-level deduplication, which means we save only
       those parts of a file that have changed.
   * - I want to update everyone about the current status of the project and
       our future plans. (from a blog post)
     - This post describes the current status of the project and future plans.

Write clear and concise sentences and paragraphs
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Users can understand wordy and complex writing, and wade through walls of text,
but they shouldn't be forced to. Use the following guidelines to help you write
clear sentences and paragraphs.

-  `Use a consistent sentence
   structure <#use-a-consistent-sentence-structure>`__
-  `Restrict sentence length <#restrict-sentence-length>`__
-  `Use only the necessary words <#use-only-the-necessary-words>`__
-  `Create short paragraphs <#create-short-paragraphs>`__

Use a consistent sentence structure
-----------------------------------

As often as possible, use the sentence structure *subject*—*verb*—*object*.
Use simple declarative sentences for descriptions, and use simple imperative
sentences for instructions. However, you can use a sentence structure that
starts with an *if* clause or places the condition before the action.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - The value is truncated only when it's stored in an integer value.
     - Only when stored in an integer variable is the value truncated.
   * - To bake a cake, follow these steps.
     - Take a look at the following procedure below to bake a simple cake.
   * - If you must monitor clients from the host, you can configure your
       settings in the directory.
     - You can configure your settings in the directory if you must monitor
       clients from the host.

Restrict sentence length
------------------------

Even when a long sentence is well written, it can be hard to follow and
understand. Try to limit sentences to 20-25 words. If you must write a longer
sentence, it should have more than one clause and the relationship between the
clauses should be clear.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - After you choose a data center, the app retrieves a list of the
       containers that are hosted within that data center. The number of files
       in each container and the approximate size of each container are
       displayed.
     - After you choose a data center, the app retrieves a list of the
       containers that are hosted within that data center, along with the
       number of files in each container and the approximate size.
   * - Select whether to overwrite files with the same name or to restore files
       to their original folders. Then, click **Next**.
     - Click the check boxes to confirm whether you would like to Overwrite
       files with the same name or restore the files to their original folders
       and then click the **Next** button.

Use only the necessary words
----------------------------

Are you using adverbs (modifiers ending in *-ly*)? If so, you can remove most
of them without changing the meaning. What about adjectives? If they aren't
necessary to the meaning, remove them. Can prepositional phrases be shortened?
Are you using empty phrases that don't clarify the content?

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - You can use the product to generate temporary URLs for files and share
       the files with other people.
     - A great feature implemented by the product is the ability to generate
       temporary URLs for files and share them with other people.
   * - Use the Control Panel to create servers easily and quickly.
     - The well-designed Control Panel is your passport to creating servers in
       an easy, fun way right away.
   * - SharePoint is the logical choice for business collaboration, content
       management, and business intelligence.
     - The flexibility, extensibility, rich feature set and ease-of-use offered
       by SharePoint make it the logical choice for many businesses when it
       comes to their Collaboration, Content Management and Business
       Intelligence needs.
   * - In an environment where the product is running, you can use the ESP
       utility to monitor and audit your backup and recovery activities across
       the enterprise.
     - In an environment where the product is installed and running on one or
       more hosts, the ESP utility enables you to monitor your backup and
       recovery activities and audit your backup and recovery practices from an
       enterprise-wide perspective.

Although shorter is usually better, be sure to include all the words that are
necessary to make the meaning of a sentence clear the first time it's read.
Include all necessary articles (*a*, *an*, *the*), prepositions, connectors,
and other syntactic cues, such as those described in
`Clarify gerunds and participles <#clarify-gerunds-and-participles>`__,
`Use restrictive and nonrestrictive clauses
correctly <#use-restrictive-and-nonrestrictive-clauses-correctly>`__,
and `Clarify pronouns <#clarify-pronouns>`__.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Empty the file.
     - Empty file.
   * - The Label option isn't supported for this file format.
     - Label option not supported for file format.

Create short paragraphs
-----------------------

Short paragraphs are easier to scan and understand. Use the following
guidelines for paragraphs:

- Cover only one idea in each paragraph.
- Limit paragraphs to four to five sentences. However, avoid having
  one-sentence paragraphs.
- Use connective or transitional words to ensure flow within and between
  paragraphs.
- When listing three or more items, use a bullet list instead of embedding the
  items in a paragraph.

The following examples show how breaking up a long paragraph by using a
list makes it easy for the user to scan the text.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - From the Job Scheduler window, you can perform the following actions:


       - Run a generated script immediately.

       - Schedule a generated script to run at a later time.

       - Track the execution of submitted jobs.

       - Manage jobs in the job queue.
     - From the Job Scheduler page, you can run a generated script immediately,
       schedule a generated script to run at a later time, track the execution
       of submitted jobs, and manage jobs in the job queue.
   * - Within the Cloud Storage App for Microsoft SharePoint, you can delete a
       single file or multiple files from a container:


       - Delete a single file by clicking the delete icon to the right of the
         file's name.

       - Delete multiple files at one time by selecting the cloud icon to the
         left of each file's name and then clicking **Delete Selected**. Rows
         that you select for deletion are highlighted with a dark gray
         background.


       When you delete a file, it's permanently removed from the
       Cloud Files container.
     - Within the Cloud Storage App for Microsoft SharePoint, you can delete a
       single file or multiple files from a container. You can delete a single
       file by clicking the delete icon to the right of the file's name. You
       can delete multiple files at one time by selecting the cloud icon to the
       left of each file's name and then clicking Delete Selected. Rows that
       you select for deletion are highlighted with a dark gray background.
       When you delete a file, it's permanently removed from the Cloud Files
       container.

Use short, familiar words and phrases
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Use short, familiar words and phrases to convey an idea clearly. Such
words and phrases are more conversational, save space, are easier to
scan, and are often easier for non-native English speakers to
understand. Use a longer word or phrase only if necessary to convey a
special meaning.

If a word has variant spellings that are equally acceptable (such as
*canceled* and *cancelled*), use the shorter spelling.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Now we test on Python 2.7.x, but we plan to support Python 3.3.x.
     - At the current time we test on Python 2.7.x, but in the future we will
       fully support Python 3.3.x.
   * - This guide is designed to get you started with the service and to answer
       your questions about the service.
     - This guide is designed to get you up and running with the service and to
       answer any questions that you may have about the service.

Use consistent terminology
~~~~~~~~~~~~~~~~~~~~~~~~~~

Use words as they are defined in a general dictionary, in an accepted
industry dictionary or style guide, or for your particular project. Each
word or phrase should have only one meaning, and should be used
consistently throughout the documentation.

-  Don't use the same word to describe two or more different concepts.
   For example, don't use *agent* to refer to both a person and a
   process.

-  If a word has both a technical meaning and a general meaning, don't
   use it to express both meanings. Instead, use a synonym for the
   general meaning. For example, use *interface* as a noun that means
   user interface. Instead of also using *interface* as a verb, use
   *interact*.

-  Don't use different words to mean the same thing. Standardize on the
   use of one word for a particular object. Technical writing isn't
   creative writing, and you shouldn't be concerned that you will bore
   users with colorless prose. Clarity is the goal, so using a
   precise set of terms consistently is required. Following is a common
   example of multiple terms that refer to the same thing:

   -  menu command *(the preferred term)*
   -  menu item
   -  menu option

-  Use a word as only one part of speech. Many words can be correctly
   used as a verb and as a noun or an adjective, such as *display*.
   However, using the same word as more than one part of speech in the
   same document can be confusing to users and translators, so avoid
   it when possible.

-  Avoid fabricated words. Examples of fabricated words are
   *marketecture* or *edutainment*. Most such words are specific to a
   single business culture and aren't understood in other cultures.

-  Standardize words and spelling across a documentation set.

-  Don't use terms with different meanings interchangeably. Some terms
   have similar but distinct meanings and shouldn't be used
   interchangeably. For example:

   -  environment, platform
   -  version, release
   -  panel, screen
   -  window, dialog box

For guidelines about specific words, see :ref:`alphabetical-list-of-terms`.

Use simple action verbs, and don't turn them into nouns
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Verbs carry the action in a sentence, and they make your documentation
come alive for users. To make the biggest impact with your writing,
use strong, simple, action verbs, and use the guidelines in this
section.

-  `Use action-oriented verbs <#use-action-oriented-verbs>`__
-  `Avoid nouns built from verbs <#avoid-nouns-built-from-verbs>`__
-  `Use the simplest tense <#use-the-simplest-tense>`__
-  `Use helping verbs accurately <#use-helping-verbs-accurately>`__
-  `Use single-word verbs <#use-single-word-verbs>`__
-  `Don't use verbs as nouns or
   adjectives <#don't-use-verbs-as-nouns-or-adjectives>`__
-  `Don't use nonverbs as verbs <#don't-use-nonverbs-as-verbs>`__
-  `Use transitive verbs transitively, not
   intransitively <#use-transitive-verbs-transitively-not-intransitively>`__
-  `Don't humanize inanimate objects <#don't-humanize-inanimate-objects>`__

Use action-oriented verbs
-------------------------

Verbs are supposed to carry the action in a sentence. However, when you use
verbs like *be*, *have*, *make*, or *do* (and their variants), or when you use
gerunds (*-ing* words), nouns carry the action and weaken the meaning. Shift
the focus from nouns to verbs by replacing weak verbs and gerunds with strong,
action-oriented verbs. Relying on verbs rather than nouns usually makes
sentences shorter, clearer, and more direct.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Rackspace **leads** the industry.
     - Rackspace **is** the industry leader.
   * - Role-Based Access Control (RBAC) **restricts** service access to
       authorized users.
     - Role-Based Access Control (RBAC) **is** a method of restricting service
       access to authorized users.
   * - If the node **can't access the Internet**, the installation process
       fails.
     - If the node **doesn't have Internet access**, the installation process
       fails.
   * - To create a server, **specify** a name, flavor, and image.
     - You create a server **by specifying** a name, flavor, and image.
   * - When you **create** a server, ...
     - When **creating** a server, ...

Avoid nouns built from verbs
----------------------------

Many nouns are built from verbs, for example, *description* and *explanation*.
Such nouns are called *nominalizations*. Sentences that include a
nominalization *and* a verb can often be simplified by changing the
nominalization back into a verb and omitting the existing verb (as shown in the
following examples).

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - The following table **describes** each of the products.
     - The following table **provides a description of** each of these
       products.
   * - **Install** the product by completing the following tasks.
     - **Perform the installation** of the product by completing the following
       tasks.
   * - The program **encrypts** user IDs and passwords.
     - The program **enables the encryption of** user IDs and passwords.

Use the simplest tense
----------------------

Simple verbs, such as verbs in the present tense, are easier to read and
understand than complex verbs, such as verbs in the progressive or
perfect tense, or verbs combined with helping verbs (such as *can*,
*may*, *might*, *must*, and *should*).

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Before you perform this task, **complete** the prerequisites.
     - Before you perform this task, you **should have completed** the
       prerequisites.
   * - To start, three ports **are** open: ssh, http, and https.
     - To start, you **are going to have** three ports open: ssh, http, and
       https.
   * - If you **use** a Red Hat distribution, iptables works a little
       differently.
     - If you **are using** a Red Hat distribution, iptables works a little
       differently.

.. _helping-verbs:

Use helping verbs accurately
----------------------------

If you need to use the following helping verbs, use them accurately and
consistently:

- **Can**: Use *can* to indicate the ability to perform an action.
- **May**: Use *may* to indicate permission.
- **Might**: Use *might* to indicate probability or possibility.
- **Must**: You can use *must* to indicate the necessity of an action. However,
  in general, use the imperative mood, which implies the subject *you* and
  doesn't require *must* but still indicates necessity.
- **Should**: Use *should* to tell users what they *ought* to do. Because
  *should* implies uncertainty, avoid using it unless you explain further.

.. list-table::
   :widths: 100
   :header-rows: 1

   * - Use
   * - You **can** customize Cloud Queues to achieve a wide range of
       performance, durability, availability, and efficiency goals.
   * - If you need space, you **may** uninstall the program.
   * - A service **might** expose endpoints in different regions.
   * - The worker **must** delete the message when work is done.
   * - To avoid losing a claim in the middle of processing a message, clients
       **should** periodically renew claims during long-running batches of
       work.

Use single-word verbs
---------------------

When possible, use single-word verbs rather than phrasal verbs (verbs
followed by prepositions or adverbs). For example, use *omit* rather
than *leave out*, or shorten *start up* to *start*. One-word verbs are
easier to understand and to translate.

If you must use a phrasal verb, keep the parts of the verb together
unless that changes the meaning of the sentence. Some acceptable phrasal
verbs are *back up*, *log in*, *set up*, *shut down*, and *work around*.

.. note::

   Don't turn a phrasal verb into a single-word verb. For
   example, don't use *login*, *setup*, or *workaround* as verbs. These
   single-word terms should be used only as nouns or adjectives.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - **Determine** the type of encryption (32-bit or 64-bit) that your
       computer uses.
     - **Figure out** the type of encryption (32-bit or 64-bit) that your
       computer uses.
   * - **Click** the link.
     - **Click on** the link.
   * - You can safely **back up a database** by using Rackspace Cloud Backup.
     - You can safely **back a database up** by using Rackspace Cloud Backup.

Don't use verbs as nouns or adjectives
---------------------------------------

If a word is defined in the dictionary as a verb, don't use it as a
noun or adjective. Some verbs that are commonly misused as nouns or
adjectives are *configure*, *compile*, *debug*, and *install*.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Correct
     - Incorrect
   * - After **installation** is completed, you can **configure** the product.
     - When you complete the **install**, you can begin the **configure**.
   * - After rubygems **is compiled**, the following message appears at the
       bottom of the output text.
     - When the **compile process** is finished, the following message appears
       at the bottom of the output text.

Don't use nonverbs as verbs
----------------------------

Don't use nouns or adjectives as verbs, and don't add verb suffixes to
abbreviations, nouns, or conjunctions.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Correct
     - Incorrect
   * - You can **reorganize** the table space.
     - You can **REORG** the table space.
   * - Verify the change **by using the ping command** to contact the server.
     - Verify the change **by pinging** the server.
   * - Some databases and search engines **insert the AND operator** between
       adjacent words in a keyword search.
     - Some databases and search engines **AND** adjacent words in a keyword
       search.
   * - **Navigate** to the new directory.
     - **CD** to the new directory.

Use transitive verbs transitively, not intransitively
-----------------------------------------------------

Transitive verbs, such as *load*, *display*, *complete*, and *execute*,
require a direct object. Intransitive verbs don't require a direct
object. Be sure to use each type of verb correctly.

To avoid using a transitive verb intransitively, you can make it passive
if the performer of the action is understood or not important.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Correct
     - Incorrect
   * - The installation program **loads** the files.

       *or*

       The files **are loaded**.
     - The files **load**.
   * - The product **displays** the available servers in the right pane.

       *or*

       The available servers **are displayed** in the right pane.
     - The available servers **display** in the right pane.
   * - After the installation **is completed**, ensure that the FTP services
       are running.
     - After the installation **completes**, ensure that the FTP services are
       running.

Don't humanize inanimate objects
--------------------------------

Be careful not to ascribe human feelings, motivations, and actions to
inanimate objects. For example, a software program doesn't know, need,
remember, see, think, understand, or want. However, it can detect,
record, require, store, check, calculate, and process.

The following anthropomorphic verbs are acceptable in the computer
industry: accept, calculate, deny, detect, interact, interpret, listen,
refuse, read, and write.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - When you reference your modules in your script by using a PHP function
       like ``include()`` or ``require()``, the server **can find** them.
     - When you reference your modules in your script by using a PHP function
       like ``include()`` or ``require()``, the server **knows where to look
       for** them.
   * - Mission-critical web-based applications and workloads **require** an HA
       solution.
     - Mission-critical web-based applications and workloads **need** an HA
       solution.
   * - The software **stores** your security profile and uses it the next time
       you log in.
     - The software **remembers** your security profile and uses it the next
       time you log in.

Clarify gerunds and participles
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Participles are verbs that end in *-ed* or *-ing* and act as modifiers. Gerunds
are verbs that end in *-ing* and act as nouns. Both types of words are useful
and acceptable, but confusion can arise if they aren't placed correctly in a
sentence. For example, the word *meeting* can be a gerund or a participle (or
even a noun) depending on its placement in a sentence. When you use gerunds and
participles, ensure that the meaning is clear.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - A job can include **metadata that schedules** the program to run at a
       specified date and time.
     - A job can include **scheduling metadata** that enables the program to
       run at a specified date and time.
   * - Public Cloud is infrastructure **that consists of** shared resources,
       deployed on a self-service basis over the Internet.
     - Public Cloud is infrastructure **consisting of** shared resources,
       deployed on a self-service basis over the Internet.
   * - Test the certificate **by using** a browser to connect to your server.
     - Test the certificate **using** a browser to connect to your server.
   * - When **you use** a load balancer with a public-facing IP address, this
       address becomes the IP address of your website.
     - When **using** a load balancer with a public-facing IP address, this
       address becomes the IP address of your website.

The last example illustrates a dangling modifier. In the "Avoid"
example, *using* doesn't have a subject, so the implied subject is
*address*, which is incorrect. If the implied subject isn't correct,
you must revise the sentence to provide a subject for the modifying
phrase.

Gerunds are used to start headings for process topics. Ensure that their
meaning is clear.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Options for editing

       *or*

       Editing of options
     - Editing options
   * - Billing for services
     - Billing services
   * - Changing the DNS settings on Windows
     - Changing DNS settings on Windows
   * - Changing a password
     - Changing passwords

.. _use-interjections-with-care:

Use interjections with care
~~~~~~~~~~~~~~~~~~~~~~~~~~~

An interjection is an emotional greeting or phrase, usually followed by
an exclamation point. For example, expressions such as *Hooray!*,
*Excuse me!*, *Sorry!*, *No thank you!*, *Oh dear!*, and *Hey, that's
mine!* are interjections.

In rare cases, an interjection might be appropriate. For example, at the
end of a procedure that targets *novice* users, you might write,
"Congratulations! You successfully created your first cloud server."

However, because the tone of an interjection can be condescending, use
them sparingly and with care.

.. _restrictive-clauses:

Use *that* and *which* correctly
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A *restrictive* clause is essential to the meaning of a sentence because it
limits the noun to which it refers. If you omit a restrictive clause, you
change the meaning of the sentence. You indicate a restrictive clause with the
relative pronoun *that* or *who*, and you don't set off a restrictive clause
with commas.

A *nonrestrictive* clause doesn't change the core meaning of the
sentence. You set off a nonrestrictive clause with commas and the
relative pronoun *which* or *who*.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Restrictive clause
     - Nonrestrictive clause
   * - He hired the man **who came from Kansas**. (Not the man from Idaho)
     - Jackhammers, **which are useful for breaking up concrete**, are on sale.
   * - Enter the user name and password **that you just created**. (Not the
       user name and password that you created last month)
     - The hourly backups are rolled into a nightly backup, **which is retained
       for two days**.

Be sure to clarify restrictive clauses, as follows:

-  Include the relative pronoun (usually *that*). You can identify
   restrictive clauses in which *that* is missing by looking for two
   successive nouns.
-  Don't substitute *which* for *that*.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Enter the user name and password **that you just created**.
     - Enter the user name and password **you just created**.

       Enter the user name and password **which you just created**.
   * - A task presents **information that a user needs** to achieve a
       specific goal.
     - A task presents **information a user needs** to achieve a specific
       goal.

       A task presents **information which a user needs** to achieve a
       specific goal.

Use pronouns sparingly
~~~~~~~~~~~~~~~~~~~~~~

Pronouns are useful, but you must ensure that their antecedents (the
words that they are used in place of) are clear, and that they (the
pronouns) don’t contribute to vagueness and ambiguity.

The following pronouns often cause problems, so use them carefully: *it*,
*this*, *there*, and *that*.

It
--

Ensure that the antecedent of *it* is clear. If multiple singular nouns
precede *it*, any of them could be the antecedent.

Avoid using *it is* (or *it's*) to begin a sentence. Such a construction hides the
real subject of the sentence.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - You can store the value and use it again later.
     - The product stores the value in the configuration file. You can use it
       again later. (The antecedent of it could be the product, the value, or
       the file.)
   * - You must close all open windows before you run the script.
     - It is important that you close all open windows before you run the
       script.

This
----

Avoid beginning a sentence with the pronoun *this*, unless you follow
*this* with a noun to clarify its meaning.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - This option causes an error when you run the program.
     - This causes an error when you run the program.

There
-----

Avoid using *there is* and *there are* as the subject of a sentence or
clause. Using *there* shifts the focus away from the real subject and
often uses unnecessary words.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - This option has no parameter
       *or*
       No parameter exists for this option.
     - There is no parameter for this option.
   * - When errors occur in the script, the product writes information to the
       message log.
     - When there are errors in the script, the product writes information to
       the message log.
   * - The Cloud Sites FTP service supports resumable uploading. If a
       connection fails during an upload, you don't need to restart the upload
       from the beginning.
     - The Cloud Sites FTP service supports resumable uploading. This means
       that if there is a connection failure during an upload, it doesn't have
       to be started from the beginning.

That
----

Although you should use *that* as a relative pronoun (see `Use
restrictive and nonrestrictive clauses
correctly <#use-restrictive-and-nonrestrictive-clauses-correctly>`__),
avoid using it as a demonstrative pronoun (which stands in for or points
to a noun). Instead, use it as an adjective and follow it with a noun.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - Use that method.
     - That is the method to use.
   * - You can also edit or delete your CNAME by managing your DNS in your
       existing tool.
     - If you want to edit or delete your CNAME, you can also do that by
       managing your DNS in your existing tool.

Use positive statements
~~~~~~~~~~~~~~~~~~~~~~~

Positive statements are easier to understand than negative statements and are
typically shorter.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - The software works properly when installed correctly.
     - The software won't work properly unless you install it correctly.
   * - Remember to involve your business users in the scheduling process.
     - Don't forget to involve your business users in the scheduling process.
   * - Sometimes you want to prevent a search engine from indexing a website.
     - It isn't uncommon in certain situations to not want to allow indexing
       of a site by a search engine.

Also, try to avoid the following negative words, using instead the
suggested alternatives. However, always be honest and transparent about
issues.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Avoid
     - Alternative
   * - damage
     - affect
   * - catastrophic
     - serious
   * - bad
     - Use *serious* or add an explanation
   * - fail
     - unable to
   * - kill
     - cancel
   * - fatal
     - serious
   * - destroy
     - remove
   * - wrong
     - incorrect, inconsistent

Use consistent references to time, space, and versions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Use the following terms consistently:

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Terms
     - Usage
     - Examples
   * - before, after
     - To locate an action in time
     - **Before** you print your document, save it.

       **After** you save your document, you can print it.
   * - following, preceding
     - To locate an item in space

       **Note**: Don't use *above*, *below*, *earlier*, *later*, *before*, or
       *after* as references to information in text. Where possible, use
       specific references. If you can't make specific references, use
       *preceding* and *following* as adjectives for elements such as
       figures and tables.
     - The **preceding** information explains how to print a document
       correctly.

       The utility analyzes the **following** information to prepare the
       report.
   * - earlier, later
     - To refer to product releases (version numbers).

       **Note**: Don't use *higher*, *lower*, *above*, *below*, *older*, or
       *newer*.
     - The required namespace kernel features aren't available in the default
       kernel shipped with Red Hat Enterprise Linux 6.4, CentOS 6.4, and
       **earlier** versions of these operating systems.

       Rackspace Private Cloud version 4.0 hasn't been tested on versions of
       Ubuntu **later** than 12.04.

Use correct punctuation
~~~~~~~~~~~~~~~~~~~~~~~

When you use correct punctuation, you help users understand what you mean
*the first time* they read the text. Following are a few basic guidelines to
apply:

-  Use a comma before the last item in a series (known as the *serial*
   comma).
-  Use a comma to separate independent clauses, and be sure to include a
   coordinating conjunction.
-  Avoid using semicolons to separate clauses. They can make long
   sentences seem even longer. You can almost always use a period in the
   place of a semicolon.
-  Don't use a slash mark (/) to present a choice among, or a series
   of, actions or objects. Rewrite the phrase to eliminate the slash
   mark. Exceptions are established terms like *client/server* and
   *read/write*.

For additional specific punctuation guidelines and examples, see
:ref:`punctuation`. For basic rules about punctuation, see a grammar book,
such as the *Harbrace College Handbook*.

.. note::

   Avoid using exclamation points, question marks, ellipses, or
   single quotation marks in text. Although these punctuation marks might
   appear in code elements, messages, literal commands, or UIs, they're rarely
   useful when writing descriptions or instructions for users. One
   exception is the use of question marks in FAQ topics.

.. _avoid-obscure-words:

Avoid obscure non-English words and abbreviations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Some non-English words and abbreviations might be unfamiliar to some users.
Latin abbreviations in particular, like *i.e.*, *e.g.*, and *etc.*, are
unnecessarily vague. The following table lists terms and abbreviations to
avoid, and their preferred alternatives.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Non-English word
     - English alternative
   * - e.g.
     - for example, such as
   * - etc.
     - and so on
   * - i.e.
     - that is
   * - per, as per
     - according to, by way of

       **Note**: The use of *per* to mean *for each* is acceptable and is
       preferable to using a slash mark.
   * - via
     - through
   * - vs.
     - versus, or an appropriate term

Write for a global audience
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Rackspace is a global company, with customers in many countries. A small
amount of content has been translated, but most has not, which means
that many customers who don't speak English as their first language
consume our English content. All of the guidelines in this topic ("Basic
writing guidelines") are designed to make content easy to understand for
all audiences, but the following guidelines will especially clarify
content for global audiences.

-  `Don't use idioms or
   colloquialisms <#don't-use-idioms-or-colloquialisms>`__
-  `Avoid metaphorical terms <#avoid-metaphorical-terms>`__
-  `Don't use humor <#don't-use-humor>`__
-  `Use jargon carefully <#use-jargon-carefully>`__
-  `Use culture-neutral language and
   examples <#use-culture-neutral-language-and-examples>`__
-  `Use culture-neutral graphics <#use-culture-neutral-graphics>`__
-  `Avoid abbreviated date formats <#avoid-abbreviated-date-formats>`__

Don't use idioms or colloquialisms
-----------------------------------

An *idiom* is an expression whose meaning can't be derived from the
literal meaning of the individual words. Some examples are *in a
nutshell*, *the bottom line*, *across the board*, and *on the fly*.

A *colloquialism* is an expression considered more appropriate to
familiar and casual conversation than to formal speech or to formal
writing. Although we might like to establish a more conversational tone
in some content, colloquialisms can be hard for non-native English
speakers to understand.

Avoid idioms and colloquialisms as often as possible.

The following table lists some idioms and colloquialisms, and provides
alternatives that you can use.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Idiom or colloquialism
     - Alternative
   * - for the most part
     - generally
   * - bear in mind, keep in mind
     - consider, remember
   * - keep an eye out for
     - look for
   * - figure out
     - determine
   * - stand for
     - represent
   * - come across
     - encounter
   * - fine tune
     - refine, customize
   * - get a feel for
     - become familiar with
   * - in light of
     - because of
   * - set aside
     - defer, allocate
   * - kind of like
     - similar to
   * - lots of
     - many
   * - what's more
     - moreover
   * - a hair smaller than
     - slightly smaller than
   * - when you're done
     - when you're finished

Avoid metaphorical terms
------------------------

A *metaphor* is a figure of speech in which a word or phrase that
denotes one kind of object or action is used in place of another to
suggest a likeness or analogy between them. Although some common
metaphors are easy even for people who don't speak English as a first
language, avoid them as often as possible.

The following table provides some examples of metaphorical terms that
can easily be replaced with one or more words.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Metaphor
     - Alternative
   * - a handful of companies
     - a few companies
   * - table a discussion
     - postpone a discussion
   * - the vanilla model
     - the standard model
   * - avoid common pitfalls
     - avoid common problems
   * - the drawback of frequent updates
     - the disadvantage of frequent updates

Don't use humor
----------------

Humor is culture specific. What might be funny in one culture might be
offensive or obscene in another culture. Humor doesn't translate well,
literally or figuratively, so don't use it.

Use jargon carefully
--------------------

*Jargon* is the specialized language of a profession. Jargon can be
useful for technical audiences, but it can be meaningless to novice
users and difficult to translate. Don't use jargon if you can
easily and correctly use a more common or familiar term, or if the
jargon obfuscates rather than clarifies the meaning. However, if the
jargon is essential to the technical meaning of the content, use it. If
the audience isn't highly technical, consider explaining any jargon
that you use.

The following table lists some jargon typically used in the high tech
industry and some possible alternatives.

.. list-table::
   :widths: 33 33 33
   :header-rows: 1

   * - Jargon
     - Alternative
     - Examples
   * - abort (verb)
     - stop, end, cancel
     - If an error occurs during data entry, the update process stops.
   * - boot, reboot (v)
     - start, restart
     - To apply your changes, restart the server.
   * - bounce (v)
     - restart
     - Restart the service.
   * - box (noun)
     - computer, server
     - The configuration specifies four servers.
   * - cache (v)
     - place in cache
     - For quick access, you can place the command in cache.
   * - debug (v)
     - resolve
     - After you resolve the problem, restart the server.
   * - dropped (adj)
     - discontinued
     - In this release, support for Windows is discontinued.
   * - execute (v)
     - run
     - Run the script.
   * - fire, fire up (v)
     - start
     - After repairs are completed, you can start the server.
   * - freeze (v)
     - stop responding
     - If the console stops responding, restart the application.
   * - grayed, grayed out (adj)
     - unavailable, dimmed
     - You can't reduce the size of a Windows server, so options for smaller
       size servers are unavailable.
   * - hang (v)
     - stop responding
     - A severe error might cause the server to stop responding.
   * - interface (v)
     - connect, communicate, interact
     - Host 1 interacts with Host 2.
   * - kill (v)
     - stop, end, terminate
     - You can terminate the process by pressing Ctrl+C.
   * - launch (v)
     - start
     - Start the application monitor in debug mode.
   * - machine (n)
     - computer, server
     - If a UFO lands in the data center, the servers stop working.

       **Note**:When referring to a virtual machine (VM), *machine* is correct.

   * - ping (v)
     - contact, alert
     - To verify the connection, use the ping command to contact the other
       server.
   * - sanity check (v)
     - test, evaluate
     - You can use a pre-existing function to evaluate the data that users
       enter.
   * - slave (n, adj)
     - subordinate, secondary (adj)
     - Database replication that uses a master database server and a secondary
       (or slave) database server provides key advantages.
   * - spin up (v)
     - create
     - If you need more capacity, create a new server.
   * - throw (v)
     - generate
     - If the program fails, an error is generated.

Use culture-neutral language and examples
-----------------------------------------

Cultural references and examples in your documentation can cause
problems for a global audience and for translation. Sounds, colors,
animals, gestures, events, and symbols don't convey the same meaning in
every culture.

-  Don't use the names of places, public figures, or holidays. If you
   must, use examples that represent a variety of cultures or that are
   internationally recognized. For example, use international cities,
   such as Paris, New York, Tokyo, London, and Hong Kong.

-  Don't use political, religious, ethnic, or historical references.

-  Don't use metaphors that are specific to one culture (for example,
   an American football metaphor).

Use generic examples that work in any target market.

If you create "named" users for extended examples or scenarios, use
names that represent a variety of ethnic backgrounds, genders, and
locations.

Use culture-neutral graphics
----------------------------

Use graphics whenever possible to present processes and complex ideas.
However, be aware of the following possible issues:

-  Some users don't typically read from left to right. If a
   graphics illustrates a sequence, make that sequence explicit by using
   numbers, arrows, or directional terms.

-  Don't rely on color alone to convey meaning. The color red, for
   example, has different meanings in different countries so could be
   interpreted differently by different users. Also, colors can have
   political or religious significance. Use neutral colors as often as
   possible.

-  Don't use a picture of a hand by itself (for example, a hand that is
   pointing). Almost every hand gesture is offensive to someone. A
   picture of a hand that is holding an item or interacting with
   something is generally acceptable.

-  Use generic or international images. Some examples are soccer players
   and equipment, generic landscapes, pens and pencils, and generic
   images of computer equipment. Avoid using images of men, women,
   flags, maps, animals, alcohol, trendy objects, historical references,
   or film, cartoon, or video characters.

Avoid abbreviated date formats
------------------------------

Date formats vary among cultures. Write out dates, unless you're
showing a literal representation as it's displayed in the software or
you need to use an abbreviation in a table or figure. If you use
abbreviations, include an explanation and use the abbreviated format
consistently.

.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Use
     - Avoid
   * - August 12, 2012
     - 8/12/2012

       8-12-12

For more guidance about writing dates, see :ref:`dates`.
