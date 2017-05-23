========================
Setting up local deconst
========================

This document takes you through the instructions for setting up deconst
on your local machine.

For more information on the Deconst staging,
see the `Deconst README <https://github.com/deconst/integrated/blob/master/README.md>`_.

Installing deconst
~~~~~~~~~~~~~~~~~~

#. Install Docker for Mac from the Managed Software Center.
#. Test everything is installed:

   .. code-block:: console

      docker --version
      docker-compose --version
      docker-machine --version

   Each command should return with the appropriate version numbers.
   For example, ``Docker version 17.03.1-ce, build c6d412e``.
#. Create a new folder for your tool work. For example,
   ``Users/alex7376/Tools``.
#. Download Kitematic: https://github.com/docker/kitematic/releases
   .. note::

      We use Kitematic for simplicity and a GUI-wrapped way of managing
      containers. However, this is  a beta product.

#. Install the Docker Toolbox for Mac:
   https://docs.docker.com/toolbox/toolbox_install_mac/
#. Fork and clone the ``deconst/integrated`` repo into your ``Tools``
   folder: https://github.com/deconst/integrated/
#. Fork and clone the ``nexus-control`` repo into your ``Tools``
   folder: https://github.com/rackerlabs/nexus-control
#. Fork and clone ``docs-rpc`` and/or ``rackspace-how-to``:

   - https://github.com/rackerlabs/docs-rpc
   - https://github.com/rackerlabs/rackspace-how-to

   .. note::

      You can use any content repo, and here are some sample ones to use

#. In your clone of ``deconst/integrated``, rename `env.example` to `env`
   and change the following lines:

   - Line 12: enter the value 1111 after the equal sign.

   - Line 16: change `deconst.horse` to `support.rackspace.com` or
     `developer.rackspace.com`.

   - Line 30: enter the path to your nexus-control repo clone
     (e.g., `/Users/laur0616/nexus-control`).

   - Line 66: enter "true" (with quotes) after the equal sign.

#. Open your terminal with two tabs or windows.
#. In both windows, navigate to the deconst/integrated directory.
#. In one terminal, run `script/up`. You will see deconst running with
   debugging turned up to full.
#. Once that terminal has stopped loading, leave it running. In the other
   terminal, run the following commands in order:

   #. `script/add-assets <path-to-nexus-control>`
      (e.g., `script/add-assets ~/nexus-control`)
   #. `script/add-<type> <path-to-content-repo>`
      (e.g., `script/add-jekyll ~/rackspace-how-to/` or
      `script/add-sphinx ~/docs-rpc/`)

#. Refresh Kitematic to see your containers. Click “View” and then
   “Refresh Container List”.
#. You should now be able to go to `localhost/<repo-link>` (e.g.,
   `localhost/how-to/`
   or `localhost/docs/private-cloud/rpc/v14/`) in your browser to see the
   delivered content.

Additional information
----------------------

If you change the control repo, run script/refresh in the same terminal
window where you ran script/add-assets. If that does not work, you can
restart everything in one of two ways:

#. Use the terminal to stop all containers. Use the second terminal window,
   and run the following command to stop all containers:

  .. code-block:: console

     docker stop $(docker ps -a -q)

#. Use Kitematic to stop all containers. You must *stop* each container, not
   restart it. Deconst needs to go up all at once to work properly.
