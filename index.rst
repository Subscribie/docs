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

--------------
Quick Start:
--------------

To add subscribie to a new project it's a good idea to add it as a git 
`submodule <https://git-scm.com/book/en/v2/Git-Tools-Submodules>`_

.. code-block:: shell
  
  pip3.6 install --user subscribiecli
  git clone git@github.com:Subscribie/subscribie.git
  cd subscribie
  pip3.6 install --user -r requirements.txt
  subscribie init
  subscribie migrate
  subscribie setconfig --TEMPLATE_BASE_DIR=<path/to/themes/dir/>
  # example subscribie setconfig --TEMPLATE_BASE_DIR=/home/fred/Downloads/subscribie/themes/
  subscribie run
  # visit http://127.0.0.1:5000
-------------------
Basic Commands:
-------------------

.. todo::
    .. code-block:: shell

     subscribie update
     subscribie subscibers # list subscribers
     subscribie new theme <theme-name> # create new theme

Visit your development site: http://127.0.0.1:5000/

Read more about :ref:`subscribie` for configuration.

Developer's Contributors Guide
==================

.. code-block:: shell

    git clone git@github.com:Subscribie/subscribie.git
    cd subscribie/
    virtualenv venv
    . venv/bin/activate
    pip install -e . # installs subscribie for local development
    export FLASK_APP=subscribie
    export FLASK_ENV=development
    subscribie run

To uninstall:

.. code-block:: shell

  # Uninstall 
  pip3.6 uninstall subscribiecli
   

User's Guide
==================

.. toctree::
   :maxdepth: 2

   jamla/jamla
   subscribie/subscribie
   themes/themes

* :ref:`search`

