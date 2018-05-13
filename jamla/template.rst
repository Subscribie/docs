.. _jamla-template:

Template
===========

A jamla template entry
   Is simply the name of the template you wish to use.


Below is an exerpt from the :ref:`jamla-latest` which shows
the default template entry:: 

	template:    
		name: jesmond 

**name**
  The name of your template. Subscribie looks for the template in 
  subscribie/templates/<name>. Template names must always be lower case.
  `string`, `mandatory`, `*default*: *jesmond*`


.. note:: In rare cases you may want to set your template to an absolute path 
          to ovveride the default location of template.

.. seealso:: :ref:`templates`
