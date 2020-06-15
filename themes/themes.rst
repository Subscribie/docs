.. _themes:

Themes
==========

Subscribie comes with an excellent default theme called `Jesmond`_. 

---------------
Getting Started
---------------

Jesmond
**********
**"jesmond"** is the name of the default theme for subscription website
builder. Jesmond is a sane default to get you up and selling quickly. Note the 
emphasis on selling. Don't waste time reinventing patterns. This theme is a
fast progessive web app
`(PWA) <https://developer.mozilla.org/en-US/Apps/Progressive>`_ which means you 
get all the benefits of modern experiences usually only found on larger
sites.

By default you have the `jesmond` theme installed, but of course you can 
create your own.

Static Assets
**************
Static assets for a theme must be placed in the 
`<theme-folder>/theme-<theme-name>/static` folder.

Every theme is stored in it's own folder named: :code:`theme-[theme-name]`.
For example, the jesmond theme is indside the :code`'themes/theme-jesmond` 
folder.

- Static assets go in the folder below, in a folder called :code:`static`.
- Template code goes into the `<theme-name>` folder below :code:`theme-[theme-name]`

::

  themes
  |
  ├── theme-jesmond
      |
      ├── jesmond
      └── static

Editing the theme
***********************
It is not recommended to edit the theme directly because your changes would
be overwitten when you update to the latest Jesmond theme. See
:ref:`create-a-theme`.

