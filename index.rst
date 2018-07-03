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

  wget https://raw.githubusercontent.com/KarmaComputing/subscribie/master/subscribie/subscribie-install.sh
  bash subscribie-install.sh

------------------
Run Subscribie:
------------------

.. code-block:: shell

  ./run.sh

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

User's Guide
==================

.. toctree::
   :maxdepth: 2

   jamla/jamla
   subscribie/subscribie
   themes/themes

* :ref:`search`

