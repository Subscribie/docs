.. _jamla_company:

Company
================

Company excerpt from :ref:`jamla-latest` :: 
 
    company:                                                                         
      name: Karma Computing                                                          
      logo: logo.svg 

A Jamla Company
   Is an `array` of common information about the company.

**name**
  Name of the company. `string`, `mandatory`

**logo**                                                                          
  Filename of the company logo. The path is assumed to be the *root*
  of the assets directory. If none is provided, templates may fallback
  to the company name. `string`, `optional`
