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

.. code-block:: shell

  git clone https://github.com/KarmaComputing/subscribie.git
  cd subscribie/hedgehog
  cp jamla.yaml.example jamla.yaml
  cp .env.example .env

Set your paths:

.. code-block:: shell

  nano .env
  DB_FULL_PATH="./data.db"                                                         
  JAMLA_PATH="./jamla.yaml"                                                        
  STATIC_FOLDER="./static/"

Run Subscribie:

.. code-block:: shell

  ./run

Visit your development site: http://127.0.0.1:5000/

User's Guide
==================

.. toctree::
   :maxdepth: 2

   jamla/jamla
   subscribie/subscribie
   themes/themes

* :ref:`search`

