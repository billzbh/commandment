Installation
============

macOS
-----

.. note:: macOS is not a recommended platform for hosting an MDM. However, you can use it to test commandment.

Manual Installation
^^^^^^^^^^^^^^^^^^^

- Install `Homebrew <https://brew.sh/>`_.
- Install Pre-requisites::

    $ brew install python3
    $ brew install uwsgi --with-python --with-python3
    $ brew install nginx

- Unpack commandment to :file:`/usr/local/commandment`.
- Use this example :download:`NGiNX configuration </_static/config/nginx-commandment.conf>`
- Use this example :download:`uWSGI configuration </_static/config/uwsgi-commandment.ini>`

.. note:: At this stage you should have an MDM Push Certificate and SSL Certificate ready so that your devices will talk
    to the MDM service. You should also decide whether to use `SCEPy <https://github.com/mosen/SCEPy>`_ for testing or
    another SCEP service such as Microsoft NDES.
