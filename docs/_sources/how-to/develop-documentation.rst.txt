How to develop documentation
============================

This tutorial shows how to setup and develop documentation.

Setup
-----

.. note::

   You need to do this first time only.

1. Install *python3.7* and *venv*

.. code-block::

   apt install software-properties-common
   add-apt-repository ppa:deadsnakes/ppa
   apt update
   apt install python3.7 python3.7-venv

2. Setup virtual environment:

.. code-block::

   python3.7 -m venv venv
   . venv/bin/activate
   pip install -r requirements.txt

Preparing environment
---------------------

.. note::

   You need to do it always when you start new terminal session.

.. warning::
   If you just made *Setup*, your environment is prepared and you can skip this step.

Activate virtual environment:

.. code-block::

   . venv/bin/activate

Building documentation
----------------------

To build documentation execute following command:

.. code-block::

   make build

This command produce HTML output and copy it to *./docs* directory.

Exiting virtual environment
---------------------------

When you will finish developing you should deactivate virtual environment.

Run command below or close terminal:

.. code-block::

   deactivate
