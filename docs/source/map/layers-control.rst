Where all geospatial files are displayed and analyzed. There are 2 main parts: layer control and toolbar.

Layers Control
--------------

Where controls and manages displayed layers like raster file or vector file.

Control Tools
=============

.. image:: ../img/control_tool_1.png
    :align: center

* Create layer: user can create new layer by add new layer or upload from ?AOI layer?, ?Tiles layer?, ?Vector file? or ?Web map service layer?

.. image:: ../img/control_tool_2.png
    :align: center

* Time serial: with images which have the data acquired, can be selected to show the chart of time series. 

* Add new group

Click icon to add new group the layers:

.. image:: ../img/control_tool_3.png
    :align: center

You can drag and drop the layer into the group.

For each group: 

* Click  icon to edit group name
* Click   icon to delete group
* Click checkbox to view all layers in group

.. image:: ../img/control_tool_4.png
    :align: center

* Save

Click icon to save workspace layer

.. image:: ../img/control_tool_5.png
    :align: center

* Delete

Click icon to delete all layers on Layers control

.. image:: ../img/control_tool_6.png
    :align: center

Display Image 
=============

Image will displayed in layer control:

.. image:: ../img/display_image_1.png
    :align: center

With icon ??? to view or not view the image, the icon ??? to zoom to layer/ image and more option can be discovered by icon ???

* The image added from Imagery will have 5 options: Rename, Properties, Tile Info, Spatial Adjustment

.. image:: ../img/display_image_2.png
    :align: center

* The raster added from Results will have 3 options: Rename, Labels control, Remove.

.. image:: ../img/display_image_3.png
    :align: center

Functions: 

* Rename: allows user change the name of layer
* Properties: will help users to change the display of images manually by using band rendering, min/max value setting and color rendering

.. image:: ../img/display_image_4.png
    :align: center

1. With customize function: users can use formulas to display images. 
2. Band rendering: have 4 choices for users: Multiband color/ Color Pallet / Singleband gray/ Singleband pseudocolor.
   Multiband color: allows users to have the composition of bands to display the image, three selected bands from the image will be used as the red, green or blue component of the color image. Allow to fetch Min and Max values for each band of the raster and scale the coloring accordingly.
   Color pallet: This is the standard render option for singleband files that include a color table, where a certain color is assigned to each pixel value. (using button “classify” by doing automatically or add manually by using the button “Add”)

.. image:: ../img/display_image_5.png
    :align: center

Singleband gray: This renderer allows you to render a single band layer with a color gradient: ‘Black to white’ or ‘White to black’  

Singleband pseudocolor: This is a render option for single-band files that include a continuous palette. with 3 modes: continuous, equal interval and quantile and 3 types of interpolation color: Exact, Discrete, Linear. (using button “classify” by doing automatically or add manually by using the button “Add”)

.. image:: ../img/display_image_6.png
    :align: center

3. A Contrast enhancement method can be applied to the values: ‘No enhancement’, ‘Stretch to MinMax’, ‘Stretch and clip to MinMax’ and ‘Clip to min max’.

* Tile Info: the information of Tile image
* Spatial Adjustment: to adjust an image to another image.
* Remove: remove layer 
* Labels control: to show the labels of results image

Display Vector
==============

Vector can be added from AOI folder, Tile layer, from PC, web map service layer or even create new layer.

* Vector added from the AOI layer by using the control tool “Create Layer” then select the AOI layer, next put the name and select the available AOI. Finally click on “Create layer”

.. image:: ../img/display_vector_1.png
    :align: center

* Vector added from the Tiles layer folder by using the control tool “Create Layer” then select the tile layer, next add the URL and finally click on “Create layer”.

.. image:: ../img/display_vector_2.png
    :align: center

* Vector added from PC by using the control tool “Create Layer” then select the vector layer, next click on File input and select the vector file from PC. Finally click on Create Layer.

.. image:: ../img/display_vector_3.png
    :align: center

* Vector added from the web map service layer by using the control tool “Create Layer” then select the web map service layer, and fill the information there before clicking on Create Layer.

.. image:: ../img/display_vector_4.png
    :align: center

The vectors are added from AOI or PC will have functions by click on icon ??? . There are 10 functions: Rename, Feature size, Style, Convert to vector, filter, table properties, Attribute  table, feature count, remove and download (.geojson).

* Rename: change the name of layer
* Style: change the style like color, opacity and width.
* Add to WMS
* Filter: allows users to define a subset of the features in the layer
* Table properties to see the attribute of layer
* Attribute table to know what type of each attribute of layer, allow to add, delete attribute.
* Feature count: to count the number of features
* Remove: remove layer
* Download: download the layer to the computer with format geojson.

The vectors added from the vectors folder will have 4 functions: Rename, Filter, Style and Remove. The functions are the same above. 

.. image:: ../img/display_vector_5.png
    :align: center

