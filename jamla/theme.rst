.. _jamla-theme:

Theme
===========

A jamla theme entry
   Is simply the name of the theme you wish to use.


Below is an exerpt from the :ref:`jamla-latest` which shows
the default theme entry:: 

	theme:    
		name: jesmond 

**name**
  The name of your theme. Subscribie looks for the theme in 
  subscribie/themes/<name>. Theme names must always be lower case.
  `string`, `mandatory`, `*default*: *jesmond*`


.. note:: In rare cases you set the theme to an absolute path, *be sure to
          also update the STATIC_FOLDER path in your .env file.*

.. seealso:: :ref:`themes`
