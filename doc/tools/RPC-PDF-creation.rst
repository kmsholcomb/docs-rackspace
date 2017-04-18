=================================
Creating a PDF file from RPC docs
=================================

.. note::
   This process is also documented at
   https://github.com/rackerlabs/docs-rpc/tree/master/pdf. It's included here
   with other tools to make sure it can be easily found. The ``pdf.sh`` is
   in https://github.com/rackerlabs/docs-rpc/tree/master/pdf.

**pdf.sh**

``pdf.sh`` is a helper script for creating PDF output from the RPC
documentation. It uses a two stage process:

#.  Build documentation into a single HTML page.

#.  Convert the HTML page to a PDF by using ``wkhtmltopdf``.

**Important**

The PDFs are current to the last updated date on the first page. You can find
the most current version in HTML format at
https://pages.github.rackspace.com/rpc-internal/docs-rpc/. You must be on the
Rackspace network to access this link.

If the content is out of date, rebuild the PDF.

Initial setup
~~~~~~~~~~~~~

``pdf.sh`` requires the ``wkhtmltopdf`` package.

Install ``wkhtmltopdf`` from the ``wkhtmltopdf`` downloads page.

Linux systems may also have ``wkhtmltopdf`` available through their package
manager.

Usage
~~~~~

Run the following command from your local ``docs-rpc`` directory:

    ``bash pdf/pdf.sh``

RPC.pdf and Handbook.pdf files are created in the ``docs-rpc/pdf`` directory.
