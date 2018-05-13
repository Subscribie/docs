.. _templates:

Templates
==========

Creating templates is easy. Every template gets passed a `Jamla` object, 
which gives you access to all information in your :ref:`jamla<jamla-latest>` 
file.

.. warning::
  Never output sensitive information from your Jamla file to your
  visitors. 

.. note::
   Ability to switch between templates is still being worked on, currently the 
   builder assumes you only have *one* template, and simply loads it from the
   `/template` base directory of your source. Issue:
   https://gitlab.com/karmacrew/hedgehog/issues/65
---------------
Getting Started
---------------

By default you have the `jesmond` template installed.

Templates are stored in your `templates` directory.

Changing the template
***********************

To change to a different template, update the name of the 
:ref:`template<jamla-template>` in your Jamla file.  
