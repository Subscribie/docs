.. _jamla-theme:

Theme
===========

.. toctree::
   :maxdepth: 2

A jamla theme entry
   Is simply the name of the theme you wish to use.


Below is an exerpt from the :ref:`jamla-latest` which shows
the default theme entry:: 

	theme:    
		name: jesmond
        static_folder: ./static

**name**
  The name of your theme. Subscribie looks for the theme in 
  subscribie/themes/<name>. Theme names must always be lower case.
  `string`, `mandatory`, `*default*: *jesmond*`

**static_folder**
  Path to static folder to serve static assets. 
  `string`, `mandatory`, `*default*: *./static*`


.. note:: You may set the theme name to an absolute path. If you do set 
          the theme name to an absolute path, be sure to *also* update the 
          STATIC_FOLDER path environment variable in your .env file.

.. seealso:: :ref:`themes`
