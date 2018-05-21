.. _subscribie:

Subscribie
===========


Subscribie is the main module which reads your :ref:`jamla` file.
It performs the following actions:

- Reads your :ref:`jamla` file
- Loads your :ref:`theme<themes>`
- Loads any modules you have defined (most have none)
- Starts Flask on localhost, listening on port 5000 by default


---------------------
Changing Configuration
---------------------

By default you don't need to change many of these options. 
Most of the options refer to paths, (such as where your :ref:`theme<themes>` 
file is) in your `.env` file.

Example:                                                                  
                                                                                    
.. code-block:: shell                                                               
                                                                                    
  nano .env                                                                         
  DB_FULL_PATH="./data.db"                                                         
  JAMLA_PATH="./jamla.yaml"                                                        
  STATIC_FOLDER="./static/"

