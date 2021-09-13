Toolbar for Analysis
--------------------

Basic toolkit: :guilabel:`mosaic tool` , :guilabel:`reclass toolset` and :guilabel:`tools` 

.. image:: ../img/toolbar_analysis.png
    :align: center 

Mosaic Tool 
===========

This tool allows the user to mosaic by manually choosing cutlines between images before mosaicing. 

Click ?? icon on toolbar to start use tool:

.. image:: ../img/mosaic_manual_tool.png
    :align: center 

Create
******

Users want to create mosaic preparation manually with given choices.

Step 1: Click Create Mosaic Preparation button  

.. image:: ../img/prepare_mosaic/create_prepare_mosaic_1.png
    :align: center 

Step 2: Type data:

1. Type Name
2. Select images from list images, at least 2 images (Search image from list)

.. image:: ../img/prepare_mosaic/create_prepare_mosaic_2.png
    :align: center 

3. Select cutline method 

.. image:: ../img/prepare_mosaic/create_prepare_mosaic_3.png
    :align: center 

- **Minimum Squared Difference**: A cutline is determined in each overlapped area between two adjacent images, with minimum square difference of gray values at the same locations of the region. 
- **Minimum Difference**: A cutline is determined in each overlapped area between two adjacent images, with minimum difference of gray values at the same locations of the region.
- **Edge**: Provides better output in urban-area mosaicking, or in images containing many linear features. The objective is to avoid placing cutlines across linear features.
- **Maximum Data**: Places cutlines on the boundary of the real image pixels, meaning that NoData pixels will be ignored when the image boundary is determined.

**Note**: Avoid placing cutlines on any of the following:

- Buildings or man-made features, because they can lean in different directions in the imagery
- Large bodies of water, because waves and the color of the water can differ among the various images
- Areas that are significantly different in color and texture, such as forests and cultivated land, because they, too, can differ image to image 

4. Check Simplify Cutlines, if not check, skip (5)
5. Type Simplification Level
6. Select Color Balancing Method: Color balancing evens out the color contrasts from one image to another to reduce the visibility of the seams and produce a mosaic that is appealing visually. There are 4 methods:

.. image:: ../img/prepare_mosaic/create_prepare_mosaic_4.png
    :align: center 

- **Bundle**: firstly, all overlapping image areas after removing anomalies in the data will compute the statistics. A bundle color adjustment (both the mean and sigma of the brightness and contrast) is applied to minimize the overall difference between all overlapping areas. Secondly, the remaining differences are modified with dodging.
- **Overlap**: computes the color-balancing histogram using only the pixels in the overlapping area of the images being added to the mosaic file.
- **Histogram**: Builds histograms for each image starting from the center of the mosaic, determines the optimum radiometry for the input image from the data then applies the transformation to the entire image.
- **Neighborhood**: using all surrounding images to modify the gain and bias of the histogram, regardless of their z-order (based on sorting order) and works iteratively to modify neighboring pixels.

7. Click Generate button

.. image:: ../img/prepare_mosaic/create_prepare_mosaic_5.png
    :align: center 

After generating, a task will be created. Wait for task success, mosaic preparation will be created. Please back to the Mosaic Preparation page to check.

Search
******

Users want to search mosaic preparation by name in the list.
Type name in search input -> Enter

.. image:: ../img/prepare_mosaic/search_mosaic.png
    :align: center 

=> Return list contains the type name.

Edit
****

Step 1: Click ?? icon 

.. image:: ../img/prepare_mosaic/edit_mosaic_1.png
    :align: center 

.. image:: ../img/prepare_mosaic/edit_mosaic_2.png
    :align: center 

Step 2: You can:

* Move layer image by drag  
* Highlight by click layer or click image directly
* Add to map  
* Zoom  
* Edit ?? : Click image directly on map -> Edit -> Click ??  icon to save

.. image:: ../img/prepare_mosaic/edit_mosaic_3.png
    :align: center 

Step 3: Click Submit button to run prepare mosaic or Back to save change.

Rename
******

Users want to Rename mosaic preparation names. Click pen icon:

.. image:: ../img/prepare_mosaic/rename_mosaic_1.png
    :align: center 

Type new name -> Click Save button

.. image:: ../img/prepare_mosaic/rename_mosaic_2.png
    :align: center 

=> Name is changed.

Run
***

Users want to run mosaic preparation to create mosaiced images.

Step 1: Click ?? icon to run:

.. image:: ../img/prepare_mosaic/run_mosaic_1.png
    :align: center 

Step 2: Type Mosaic image name -> Click Submit button

.. image:: ../img/prepare_mosaic/run_mosaic_2.png
    :align: center 

Step 3: Confirm pay cost

=> => Task will be created in Tasks, wait task success, check result in Imagery.

Delete
******

Users want to delete Mosaic Preparation.
Click ?? icon of Mosaic Preparation you want delete.
Then Click the Delete button to confirm delete.

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

There are 4 types of tools: ARD, Vector toolkit, Unsupervised and Result toolkit.

* **ARD Toolkit**: includes the tool for analysing raster/ images. 

Click ?? icon to start use tools:

.. image:: ../img/image_tools/ard_toolkit_1.png
    :align: center 

Select tool:

.. image:: ../img/image_tools/ard_toolkit_2.png
    :align: center 
.. image:: ../img/image_tools/ard_toolkit_3.png
    :align: center 

Select type ARD:

.. image:: ../img/image_tools/ard_toolkit_4.png
    :align: center 
.. image:: ../img/image_tools/ard_toolkit_5.png
    :align: center 

For more informations about tool, click ?? icon.

Advanced Mosaic
****************

This tool support merge/ combination list of images into a single image automatically

Step 1: Type input

1. Type name
2. Select images from list images (type search input to search image)

.. image:: ../img/image_tools/advanced_mosaic_1.png
.. image:: ../img/image_tools/advanced_mosaic_2.png

Step 2: Click Submit button

.. image:: ../img/image_tools/advanced_mosaic_3.png
    :align: center

Step 3: Click Confirm to pay cost

.. image:: ../img/image_tools/confirm_pay_cost.png
    :align: center

=> Task will be created. When task is success, please check result in menu **Imagery**

Align Pixel
***********

This tool is able to take several rasters as input and to align them perfectly, that means:

- reproject to the same CRS,
- resample to the same cell size and offset in the grid,
- clip to a region of interest,
- rescale values when required.

1. Type name
2. Select image from list images (only one image)
3. Select reference image (only one image):  

.. image:: ../img/image_tools/align_pixel_1.png
    :align: center

Aspect
******

Calculates the aspect of the Digital Terrain Model in input. The final aspect raster layer contains values from 0 to 360 that express the slope direction, starting from north (0°) and continuing clockwise.

1. Type name
2. Select image from list images (only one image)
3. There are 4 option:
    - Trigonometric: trigonometric angle instead of azimuth. Thus 0° means East, 90° North, 180° West, 270° South
    - Zero for flat:Return 0 for flat areas with slope=0, instead of -9999 
    - Compute Edges: Generates edges from the elevation raster
    - Use Zevenbergen Thorne formula instead of the Horn's one: The literature suggests Zevenbergen & Thorne to be more suited to smooth landscapes

.. image:: ../img/image_tools/aspect_1.png
    :align: center

Cloud Free Mosaic
*****************

It will help users remove clouds in an area if there are collections of overlapping images.

Step 1: Type input

- Type name
- Select images (images must overlap)
- There are two options:
    - Sort by acquired date (asc) (default)
    - Sort by cloud percentage

.. image:: ../img/image_tools/cloud_free_mosaic_1.png
    :align: center

Dem Extraction
**************

A DSM (also referred to as a DEM) extracted from stereo images represents the earth’s surface and includes all objects on it. 

1. Type name
2. Select images: select stereo images

.. image:: ../img/image_tools/dem_extraction_1.png
    :align: center

Dem Super Resolution
********************

Increasing the resolution of DEM images.

1. Type name
2. Select image (only one image): 

.. image:: ../img/image_tools/dem_super_resolution_1.png
    :align: center

Down Scale
**********

Improve the resolution of the image from low to high resolution.

1. Type name
2. Select image
3. There are two level:
    - 2: means an increase in spatial resolution in double. For example from resolution 10m, downscale will improve the spatial resolution to 5m.
    - 4: means increasing in spatial resolution four times.

.. image:: ../img/image_tools/down_scale_1.png
    :align: center

Hillshade
*********

The hillshade is calculated by using DEM image and the sun position

1. Type name
2. Select image
3. Type z factor: Vertical exaggeration used to pre-multiply the elevations
4. Type scale: Ratio of vertical units to horizontal. If the horizontal unit of the source DEM is degrees (e.g Lat/Long WGS84 projection), you can use scale=111120 if the vertical units are meters (or scale=370400 if they are in feet)
5. Type Azimuth of the light:Azimuth of the light, in degrees. 0 if it comes from the top of the raster, 90 from the east, …
6. Type Altitude of the light: Altitude of the light, in degrees. 90 if the light comes from above the DEM, 0 if it is raking light
7. There are two options:
    - Compute Edge
    - Use Zevenbergen Thorne formula instead of the Horn's one
8. Select Shading type 
    - Combined: combined shading, a combination of slope and oblique shading
    - Multidirectional: multidirectional shading, a combination of hill shading illuminated from 225 deg, 270 deg, 315 deg, and 360 deg azimuth.

.. image:: ../img/image_tools/hill_shade_1.png
.. image:: ../img/image_tools/hill_shade_2.png

Image Resampling
****************

Decrease the resolution of the image. Change image from high resolution to low resolution.

1. Type name
2. Select image
3. Type level: (if you choose level 2, the spatial resolution will decrease double for example raw data has 5m resolution, after resampling with level 2, the resolution will be 10m)

.. image:: ../img/image_tools/image_resampling_1.png
    :align: center

Mosaic
******

This tool supports merge/ combination list of images into a single image automatically. It is similar to advanced mosaics with different algorithms.

Orthorectify
************

Orthorectify is the process of removing the effects of terrain and sensor creating a planimetrically correct image. The image will match the spatial by considering location, elevation and sensor information.
 
5. Matching band
6. Number of GCPs: Type the number of points that you want to collect over each image
7. Minimum acceptance score: enter a value from 0-1 which defines the minimum correlation score that will be considered a successful match.
8. There are two Matching method:
    - FFTP: Fast Fourier Transform Phase Matching: when two images have a relative shift between them, the result is a phase difference in the Fourier domain. FFTP determines the shift between images using this phase difference.
    - NCC: Normalized Cross Correlation. This method finds the relative shift between two images by finding the shift that produces the maximum cross-correlation coefficient of the gray values in the images. 
9. Search radius: type a number to define the search radius around the kernel

.. image:: ../img/image_tools/orthorectify_1.png
.. image:: ../img/image_tools/orthorectify_2.png

Pansharpening
*************

Pansharpen will use a panchromatic image to sharpen the multispectral image to create a high resolution color image.

.. image:: ../img/image_tools/pansharpening_1.png
    :align: center

Polygonize
**********

This tool is specially designed for post processing of the Farmboundary model. The input file is the results of farm boundary model.

.. image:: ../img/image_tools/polygonize_1.png
    :align: center

Raster Clip
***********

Clip the Raster using the mask layer

.. image:: ../img/image_tools/raster_clip_1.png
    :align: center

Slope
*****

Calculate the slope from the DEM image. The slope is the angle of inclination of the terrain and is expressed in degrees

.. image:: ../img/image_tools/slope_1.png
    :align: center

Stack
*****

Layer stacking is a process for combining multiple images with same extent into a single image.

.. image:: ../img/image_tools/stack_1.png
    :align: center

Visual Imagery
**************

To convert an image to data type unit 8 with reference image or not.

.. image:: ../img/image_tools/visual_1.png
    :align: center

Zonal
*****

Calculates statistics of a raster layer for each feature of an overlapping polygon vector layer.

.. image:: ../img/image_tools/zonal_1.png
    :align: center

In Algorithm, there are 4 options:

- Min: Determines the smallest value of all cells in the value raster that belong to the same zone as the output cell
- Mean: Determines the mean of all cells in the value raster that belong to the same zone as the output cell
- Max: Determines the largest value of all cells in the value raster that belong to the same zone as the output cell
- Most value: Determines the most value of all cells in the value raster that belong to the same zone as the output cell

Step 2: Click Confirm button

Step 3: Confirm to pay cost

**Result toolkit**: includes the tool for analysing raster results.

.. image:: ../img/image_tools/result_toolkit.png
    :align: center

Crop Scout
**********

Step 1: Type input: (You can check raster results in Results or Imagery)

.. image:: ../img/image_tools/crop_scout_1.png
    :align: center

Step 2: Click Tool setting button -> Select raster band:

.. image:: ../img/image_tools/crop_scout_2.png
.. image:: ../img/image_tools/crop_scout_3.png

Step 3: Click Confirm button

The Task will be created in Tasks. Wait for task success, check result.

Reclassification
****************

Step 1: Type input

.. image:: ../img/image_tools/reclassification_1.png
    :align: center

Step 2: Click “Tool setting” button

1. Click color box to change color for each class
2. Change name for each class
3. Change value for each class

.. image:: ../img/image_tools/reclassification_1.png
    :align: center

Step 3: Click Apply button. The Task will be created in Tasks. Wait for task success, check result.

Morphology
**********

This help users in post processing to eliminate the small area and fill the hole

Step 1: Type input

.. image:: ../img/image_tools/morphology_1.png
    :align: center

Step 2: Click “Tool setting” button -> Type epsilon

.. image:: ../img/image_tools/morphology_2.png
    :align: center

Step 3: Click Confirm button. The Task will be created in Tasks. Wait for task success, check result.

Vectorization
*************

Step 1: Type input

.. image:: ../img/image_tools/vectorization_1.png
    :align: center

Step 2: Click “Tool setting” button -> Type epsilon

.. image:: ../img/image_tools/vectorization_2.png
    :align: center

Step 3: Click Confirm button. The Task will be created in Tasks. Wait for task success, check result.


