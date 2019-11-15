.. _install-subscribiecli:

Install Subscribie CLI
======================

The Subscribie command-line tool, allows you to run commands 
against a local subscribie site. It allows you to:

- Initialise a new Subscribie project
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

.. note:: If you're on a Mac, make sure python3 (or python3.6, or python3.7)
          is in your PATH. MacOS 10.14 and above defaults to zsh so you need
          to edit your ~/.zshrc file to ensure python 3 (or above) is in your 
          path. For example, at the bottom of your :code:`~/.zshrc` file:

          .. code-block:: shell

             nano ~/.zshrc
             # Add python 3.7 to PATH:
             export PATH=$PATH:/Users/karabeen/Library/Python/3.7/bin
          
          Change accordingly to the python version you have installed on your
          mac (you must have at least python version 3). For bash, edit your
          :code:`~/.bashrc` file with the same edit at the bottom.

Install Subscribie CLI
-----------------------

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
    init       Initialise a new subscribie project
    initdb     Initialise the database
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
    init       Initialise a new subscribie project
    initdb     Initialise the database
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
