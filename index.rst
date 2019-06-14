
.. Subscription Website Builder documentation master file, created by
   sphinx-quickstart on Thu May 10 18:31:14 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Subscription Website Builder's Documentation
========================================================

                                                                                                                                                                 
.. sidebar:: What you get

	* Take recurring payments using direct debit
	* Instant payments for up-front costs
	* A simple workflow
                                                                                 

Subscription Website Builder (Subscribie) makes is easy for you to design and 
build a subscription based website. We've built all the complicated stuff for
you.

A simple workflow:

1. Customer chooses a package
2. Customer enters contact info
3. Take one-off/monthly payments (or both)

.. _quickstart:

-----------------------
Quickstart: Run locally
-----------------------

Requirements:

- Python 3 or greater (Do :code:`python --version` to find out your version)

  - `Install python <https://www.python.org/downloads/>`_.

- Pip (python package installer) 

  - `Install Pip <https://pip.pypa.io/en/stable/installing/#installation>`_.

Get the subscribie code:
`````````````````````````
.. code-block:: shell
  
  pip3.6 install --user subscribiecli
  git clone git@github.com:Subscribie/subscribie.git
  cd subscribie
  pip3.6 install --user -r requirements.txt
  subscribie init
  subscribie migrate

Set theme path directory:
``````````````````````````
Now set the full path (with terminating slash) to the directory 
of the themes directory. By default this is a subdirectory of the
subscribie folder, but you can place themes anywhere on your filesystem.

.. code-block:: shell

  subscribie setconfig --TEMPLATE_BASE_DIR=<path/to/themes/dir/>
  # example subscribie setconfig --TEMPLATE_BASE_DIR=/home/fred/Downloads/subscribie/themes/

Run subscribie locally:
```````````````````````

.. code-block:: shell

  export FLASK_DEBUG=1 # See theme changes on every refresh
  subscribie run
  # visit http://127.0.0.1:5000

Visit your development site: http://127.0.0.1:5000/

Read more about :ref:`subscribie` for configuration.

-------------------
Basic Commands:
-------------------

The most useful two commands are: 

- :code:`subscribie --help` (shows help menu)
- :code:`subscribie --setconfig --help` (for changing config)

.. code-block:: shell

  Usage: subscribie [OPTIONS] COMMAND [ARGS]...

  Options:
    --help  Show this message and exit.

  Commands:
    init       Initalise a new subscribie project
    initdb     Initalise the database
    migrate    Run latest migrations
    newtheme   Create new theme
    run        Run subscribie
    setconfig  Updates the config.py which is stored in instance/config.py...

-------------
To uninstall:
-------------

.. code-block:: shell

  # Uninstall 
  pip3.6 uninstall subscribiecli
   

User's Guide
==================

.. toctree::
   :maxdepth: 2

   concepts/concepts
   tasks/tasks
   jamla/jamla
   subscribie/subscribie
   themes/themes

* :ref:`search`

