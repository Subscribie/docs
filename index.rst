
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

Quickstart: Run locally
-----------------------

.. code-block:: shell

  git clone https://github.com/Subscribie/subscribie.git                         
  cd subscribie                                                                  
  cp .env.example .env # Copy default .env settings (look at it)                 
  virtualenv -p python3 venv # Create a python3.x virtualenv                     
  . venv/bin/activate # Activate the virtualenv                                  
  pip install -r requirements.txt # Install requirements                         
  export FLASK_APP=subscribie                                                    
  export FLASK_DEBUG=1
  flask initdb # (optional) initalize the database with dummy data
  flask run # Run the app 

  Now visit http://127.0.0.1:5000 

User's Guide
==================

.. toctree::
   :maxdepth: 2

   get-started/index
   concepts/concepts
   tasks/tasks
   subscribie/subscribie
   themes/themes

* :ref:`search`

