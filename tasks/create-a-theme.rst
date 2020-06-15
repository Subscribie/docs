.. _create-a-theme:

Create a Subscribie theme
===========================

.. toctree::
  :maxdepth: 2

How to create a frontend theme for Subscribie.

Before you begin
-----------------

Make sure you have already:

- :ref:`install-subscribiecli`

Create a new theme using Subscribie cli
----------------------------------------

1. Go to your root subscribie folder
`````````````````````````````````````

.. code-block:: shell

   cd subscribie 

2. Create a new theme, based on jesmond theme
``````````````````````````````````````````````

.. code-block:: shell

   subscribie newtheme --name mynewtheme --base jesmond

The :code:`subscribie newtheme` command will take a copy of 
the latest jesmond theme (from github) and rename it to the 
name you gave. 

Find your new theme in your themes directory.
If you want to use another theme as a base, look at the themes
already in the Subscribie github organisation: https://github.com/Subscribie?utf8=%E2%9C%93&q=theme-&type=&language=

3. Edit your :code:`.env` file to the new theme name
```````````````````````````````````````````````````````````

Take out the existing theme name and src for jesmond, and replace
it with your own, removing the src attribute. For example:

.. code-block:: shell
  
  THEME_NAME=mytheme

4. Run your new theme
``````````````````````

Run your subscribie site locally. During the output, you should
see your theme name has changed to :code:`mynewtheme`:

.. code-block:: shell

  export FLASK_DEBUG=True
  subscribie run
  ...
  ...
  Theme name is: mytheme
  ...

Make some changes to your theme, and an reload. It will look 
exactly the same as jesmond to start with.
