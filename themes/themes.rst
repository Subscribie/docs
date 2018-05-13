.. _themes:

Themes
==========

Subscribie comes with an excellent default theme called `Jesmond`_. Every 
theme gets passed a `Jamla` object, which gives you access to all information 
in your :ref:`jamla<jamla-latest>` file.

.. warning::
  Never output sensitive information from your Jamla file to your
  visitors. 

---------------
Getting Started
---------------

Jesmond
**********
**"jesmond"** is the name of the default theme for subscription website
builder. Jesmond is a sane default to get you up and selling quickly. Note the 
emphasis on selling. Don't waste time reinventing patterns. This theme is fast a
fast progessive web app
`(PWA) <https://developer.mozilla.org/en-US/Apps/Progressive>`_ which means you 
get all the benefits of fast modern experiences usually only found on larger
sites

By default you have the `jesmond` theme installed, but of course you can 
create your own by editing your jamla :ref:`jamla-theme` setting to point to
another theme.

Static Assets
**************
Static assets must be placed in `subscribie/static` above the template folder:

::

	subscribie
	├── static
	│   └── logo.svg
	└── templates
		└── jesmond

Editing the theme
***********************
It is not recommended to edit the theme directly because your changes would
be overwitten when you update to the latest Jesmond theme. Instead you would 
create your own theme.

Changing the theme
***********************

To change to a different theme, update the name of the :ref:`jamla-theme` in your Jamla file.  


