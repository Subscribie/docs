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
Configure Subscribie:
--------------

.. code-block:: shell

  git submodule add git@github.com:KarmaComputing/subscribie.git
  cp subscribie/hedgehog/jamla.yaml.example jamla.yaml
  mv subscribie/hedgehog/.env.example subscribie/hedgehog/.env
  #Set your jamla.yaml location by editing the .env file
  python createdb.py # Initalize database
  for file in migrations/*; do ./$file -up ; done # run migrations

------------------
Run Subscribie:
------------------

.. code-block:: shell

  ./run

Visit your development site: http://127.0.0.1:5000/

Read more about :ref:`subscribie` for configuration.

User's Guide
==================

.. toctree::
   :maxdepth: 2

   jamla/jamla
   subscribie/subscribie
   themes/themes

* :ref:`search`

