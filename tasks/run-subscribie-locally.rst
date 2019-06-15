.. _run-subscribie-website-locally:

Run a Subscribie website locally
=======================

Clone the Subscribie codebase
`````````````````````````
.. code-block:: shell
  
  git clone git@github.com:Subscribie/subscribie.git
  cd subscribie
  pip3.6 install --user -r requirements.txt
  subscribie init # Sets up initial project
  subscribie migrate # Migrates database

Set theme path directory
``````````````````````````
Now set the full path (with terminating slash) to the directory
of the themes directory. By default this is a subdirectory of the
subscribie folder, but you can place the themes folder anywhere 
you line on your filesystem.

.. code-block:: shell

  subscribie setconfig --TEMPLATE_BASE_DIR=<path/to/themes/dir/>
  # example subscribie setconfig --TEMPLATE_BASE_DIR=/home/fred/Downloads/subscribie/themes/

Run Subscribie locally
```````````````````````

.. code-block:: shell

  export FLASK_DEBUG=1 # See theme changes on every refresh
  subscribie run
  # visit http://127.0.0.1:5000

Visit your development site: http://127.0.0.1:5000/

Read more about :ref:`subscribie` for configuration.


