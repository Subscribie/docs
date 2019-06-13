.. _subscribie:

Subscribie
===========


Subscribie is the main module which reads your :ref:`jamla` file.
It performs the following actions:

- Reads your :ref:`jamla` file
- Loads your :ref:`theme<themes>`
- Loads any modules you have defined (most have none)
- Starts Flask on localhost, listening on port 5000 by default


---------------------
Changing Configuration
---------------------

By default you don't need to change many of these options. 
Most of the options refer to:

- Paths
- Modules

To change settings use the :code:`subscribie` command line utility.

- View the setconfig help menu: :code:`subscribie --setconfig --help`
- View basic help menu: :code:`subscribie --help`

Example:                                                                  
                                                                                    
.. code-block:: shell                                                               

  subscribie setconfig --help

  Usage: subscribie setconfig [OPTIONS]

    Updates the config.py which is stored in instance/config.py :param config:
    a dictionary

  Options:
    --JAMLA_PATH TEXT               full path to                jamla.yaml
    --SECRET_KEY TEXT               Random key for flask                sessions
    --TEMPLATE_FOLDER TEXT          Path to theme                folder
    --STATIC_FOLDER TEXT            Path to static assets                folder
    --UPLOADED_IMAGES_DEST TEXT     Path to image               upload folder
    --DB_FULL_PATH TEXT             Path to database
    --SUCCESS_REDIRECT_URL TEXT     Mandate complete redirect url
    --THANKYOU_URL TEXT             Thank you url (journey complete url)
    --MAIL_SERVER TEXT              Mail server hostname or IP
    --MAIL_PORT INTEGER             Email submission port
    --MAIL_DEFAULT_SENDER TEXT      Default mailserver from
    --MAIL_USERNAME TEXT            Mailserver username
    --MAIL_PASSWORD TEXT            Mailserver password
    --MAIL_USE_TLS TEXT             Mailserver use TLS
    --EMAIL_LOGIN_FROM TEXT         Default email from
    --GOCARDLESS_CLIENT_ID TEXT     GoCardless client id               (not
                                    needed by default, unless doing a partner
                                    integration)
    --GOCARDLESS_CLIENT_SECRET TEXT
                                    GoCardless client                secret (not
                                    needed by default, unless doing partner
                                    integration
    --TEMPLATE_BASE_DIR TEXT        Set template base dir
    --help                          Show this message and exit.
