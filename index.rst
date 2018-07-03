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

  git init # Start a git project (you might already have one, skip if you do)
  git submodule add git@github.com:KarmaComputing/subscribie.git
  cp subscribie/subscribie/jamla.yaml.example jamla.yaml
  cp subscribie/subscribie/.env.example subscribie/subscribie/.env
  #Set your jamla.yaml location by editing the .env file
  sed -i s#JAMLA_PATH.*#JAMLA_PATH=\"$PWD/jamla.yaml\"#g subscribie/subscribie/.env
  # Copy over default templates
  cp -R subscribie/subscribie/templates ./
  cp -R subscribie/subscribie/static ./
  # Set template fallback base dir folder
  sed s#TEMPLATE_FOLDER=.*#TEMPLATE_FOLDER=\"$PWD/templates/\"#g subscribie/subscribie/.env
  # Set static dir
  sed -i s#static_folder:.*#static_folder: \"$PWD/static/\"#g jamla.yaml 
  python subscribie/subscribie/createdb.py # Initalize database
  # Run database migrations
  for file in subscribie/subscribie/migrations/*; do ./$file -up -db "$PWD"/data.db; done
  cp subscribie/subscribie/run.sh ./
  sed -i s#FLASK_APP=#FLASK_APP=$PWD/subscribie/subscribie/#g run.sh
  sed -i s#HEDGEHOG_ENV=.*#HEDGEHOG_ENV=$PWD/subscribie/subscribie/.env#g run.sh

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

