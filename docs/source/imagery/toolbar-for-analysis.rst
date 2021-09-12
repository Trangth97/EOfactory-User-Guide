Toolbar for Analysis
--------------------

Basic toolkit: mosaic tool, reclass toolset and tools 

.. image:: ../img/toolbar_analysis.png
    :align: center 

Mosaic Tool 
===========

This tool allows the user to mosaic by manually choosing cutlines between images before mosaicing. 

Click ???  icon on toolbar to start use tool:

.. image:: ../img/mosaic_manual_tool.png
    :align: center 

?????

Reclass Toolset
===============

Reclass toolset will reclassify (or change) the value in a raster- a range of value pixels will be reclassified or a single pixel (unique) will be assigned to another value.

You can choose image first, then click   icon or click  icon, then select image.

* Choose image -> Click   icon:

Step 1: Select band (Only one, you can search if there are many bands)

.. image:: ../img/reclass_toolset_1.png
    :align: center 

Step 2: Click Classify button

.. image:: ../img/reclass_toolset_2.png
    :align: center 

Step 3: Type input:

- Select mode

  -	Standard Deviation: the method shows you how much a feature’s attribute value varies from mean. Class breaks are created with equal value ranges that percentage of the standard deviation using mean value and the standard deviation from the mean
  - Equal interval: the method divides the range of values into equal-sized subranges.
  - Quantile: the method will assign the same number of values to each class. There are no empty classes or classes with too few or too many values. This method works well with the linearly distributed data.
- Type Amount of value (If mode is Standard Deviation, the default Amount of value will be 6)

.. image:: ../img/reclass_toolset_3.png
    :align: center 

Step 4: Click Classify button

.. image:: ../img/reclass_toolset_4.png
    :align: center 

After click Classify button, please see Histogram and Break Values based mode and amount of value

.. image:: ../img/reclass_toolset_5.png
    :align: center 

Step 5: Click Confirm button

.. image:: ../img/reclass_toolset_6.png
    :align: center 

Step 6:

* You  can add Max value - Min value - Value

.. image:: ../img/reclass_toolset_7.png
    :align: center 

Type new data

.. image:: ../img/reclass_toolset_8.png
    :align: center 

or you can edit by type directly

or delete by click ??? icon

* You can Revert values

.. image:: ../img/reclass_toolset_9.png
.. image:: ../img/reclass_toolset_10.png

* You can Clear all values

.. image:: ../img/reclass_toolset_11.png
    :align: center 

* Default: No data value equal 0. If you want to change No data value, type input directly. And click checkbox if you want to change miss value to No data

.. image:: ../img/reclass_toolset_12.png
    :align: center 

* Click Unique if you want each old value to correspond to a unique new value

.. image:: ../img/reclass_toolset_13.png
    :align: center 

Step 7: Click Submit button

.. image:: ../img/reclass_toolset_14.png
    :align: center 

Type name -> Click Confirm button

.. image:: ../img/reclass_toolset_15.png
    :align: center 

=> Tasks will be created in Tasks. Wait task was successful, please check at Imagery with the correct name.

Tools 
=====

?????
