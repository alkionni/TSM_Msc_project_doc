.. PINNs documentation master file, created by sphinx-quickstart on Sun Sep 20 12:39:03 2026. You can adapt this file completely to your liking, but it should at least contain the root `toctree` directive.

Transient Surrogate Model documentation
===================

.. Add your content using ``reStructuredText`` syntax. See the `reStructuredText <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_documentation for details.

----------------------------------------------------------------
Circuit Simulation Machine Learning Model for Transient Analysis
----------------------------------------------------------------

A framework for generating the dataset, training, evaluating, testing and deploying neural network models for
analog circuit analysis' simulations prediction.

Contains 2 circuits: An Operational Amplifier and a Low Dropout Regulator for modeling the AC and transient analysis
respectively.

Installation:
-------------
To install the project after cloning you need to run poetry install.

How to use:
-------------
For LDO:
   1. Generate the dataset using the 'generate_simulations' script.
   2. Update the dataset path in LDO/config.py file.
   3. Choose your parameters from the config.py file, like whether to use LDR or LNR.
   4. Train a model with the train.py file.
   5. Test the model with the inference.py file.

For OPAMP:
   1. Generate the dataset using the 'generate_simulations' script.
   2. Update the dataset path in OP_AMP/utils/dataset.py file.
   3. Choose your parameters from the main.py file, like whether to use gain or phase.
   4. Train and test a model with the main.py file.

Docs
----
To view the project documentation, run ``make html`` from ``/docs`` directory in your terminal.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   modules
