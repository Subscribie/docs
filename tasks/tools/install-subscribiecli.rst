.. _install-subscribiecli:

Install Subscribie CLI
======================

The Subscribie command-line tool, allows you to run commands 
against a local subscribie site. It allows you you:

- Initalise a new Subscribie project
- Run a subscribie site locally 
- Change subscribie config settings
- Create new themes using existing themes as a starting point

Before you begin
------------------

You must be using at least :code:`python` version 3 and have the
python package manager :code:`pip` installed.

- Python 3 or greater (Do :code:`python --version` to find out your version)

  - `Install python <https://www.python.org/downloads/>`_.

- Pip (python package installer)

  - `Install Pip <https://pip.pypa.io/en/stable/installing/#installation>`_.


.. code-block:: shell
  :name: Install subscribiecli
  
  pip3.6 install --user subscribiecli

Verify subscribie cli installation
-----------------------------------

When you type :code:`subscribie` in your terminal, you should see
output similar to:

.. code-block:: shell
  :name: Verify subscribie cli install

  subscribie
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

-------------------
Basic subscribie Commands:
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
Uninstall subscribie cli
-------------

.. code-block:: shell

  # Uninstall 
  pip3.6 uninstall subscribiecli

What's next
------------

- :ref:`run-subscribie-website-locally`