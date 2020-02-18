.. _create-a-module:

Create a Subscribie module
==============================

.. toctree::
  :maxdepth: 2

Name your module
---------------------

Create a module named: module-<name-of-module> 
e.g. If your creating a module called "postage" name your module: 
"module-postage".


Create the following file strucutre:
--------------------------------------

.. code-block:: shell

    module-postage./
    ├── __init__.py
    ├── README.md
    └── templates/


You will typically need at least the following imports in your __init__.py:


.. code-block:: shell

    from flask import (Blueprint, render_template, abort, request, redirect)
    from jinja2 import TemplateNotFound
    from subscribie.db import get_jamla
    from subscribie.auth import login_required


Declare module
--------------------

In your __init__.py declare the module as a Flask blueprint (read about flask blueprints).

.. code-block:: shell

    module_postage = Blueprint('iframe_postage', __name__, template_folder='templates')


Create an index page for your module (e.g. a settings page)
-------------------------------------------------------------

Every module should have an index page, this will appear 
on the shop admin dashboard allowing the user to configure
and access your module if needed.

.. code-block:: shell

    @module_postage.route('/module_postage/index') # Define a module index page
    @module_postage.route('/show-module-postage-settings-index')
    @login_required
    def get_module_postage_index():
      """Index page for module_postage settings."""

      try:
        return render_template('module_postage_index.html', jamla=get_jamla())
      except TemplateNotFound:
        abort(404)
