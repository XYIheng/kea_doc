Kea doc
=======================================
https://kea-doc.readthedocs.io/en/latest/


Developer Tutorial
======================================

**Set up**

.. code-block:: bash
    git clone git@github.com:XYIheng/kea_doc.git

    cd kea_doc/docs

    pip install -r requirements.txt

**Use vscode RST previewer**

Add the following extension to vscode:

`reStructuredText <https://marketplace.visualstudio.com/items?itemName=lextudio.restructuredtext>`_

`reStructuredText Syntax highlighting <https://marketplace.visualstudio.com/items?itemName=trond-snekvik.simple-rst>`_

`Esbonio <https://marketplace.visualstudio.com/items?itemName=swyddfa.esbonio>`_

Install Esbonio server

.. code-block:: bash
    
    pip install esbonio

reboot vscode to apply the changes.

**build html**

.. code-block:: bash

    cd kea_doc/docs

    # You should delete the build dir every time you modify the file structure of the project
    # Or the cache will affect the previewer of the esbonio extension.
    rm -r build

    make html

Template for the Read the Docs tutorial
=======================================

This GitHub template includes fictional Python library
with some basic Sphinx docs.

Read the tutorial here:

https://docs.readthedocs.io/en/stable/tutorial/
