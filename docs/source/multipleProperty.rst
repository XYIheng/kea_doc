Run multiple properties together
====================================

The random and main path guided exploration strategies by default validate one property of an app at one run.
When multiple properties of an app are available,these two strategies can validate any subset of these properties together.
One benefit is that we can improve the efficiency of validating properties.
Another benefit is that the interaction scenarios of multiple properties provide a partial model of the app.
This partial model enables us more likely to reach deeper app states during testing.

Specifically, to validate multiple properties together, the random strategy would check
whether multiple properties’ preconditions are satisfied, and randomly select one property for checking.
The main path guided exploration strategy would randomly select one property as the target,
and perform guided exploration along its main path. When every state on this main path has been explored,
this strategy would randomly select another property as a new target.
In addition, this strategy would randomly select a property for check when multiple properties’ preconditions are satisfied.

Suppose we have several properties in different files, we can run them together by specifying multiple files in the command line.

.. code-block:: console

   kea -f [property_file_name1] [property_file_name2] -a [apk_file_name]
