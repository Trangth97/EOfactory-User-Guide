Tools
-----

Buffer
======

This algorithm computes a buffer area for all the features in an input layer, using a fixed or dynamic distance. The segments parameter controls the number of line segments to use to approximate a quarter circle when creating rounded offsets. The end cap style parameter controls how line endings are handled in the buffer. The join style parameter specifies whether round, miter or beveled joins should be used when offsetting corners in a line.The miter limit parameter is only applicable for miter join styles, and controls the maximum distance from the offset curve to use when creating a mitered join.

Step 1: Type input:

1. Type **Name**
2. Select **Vector** from Vectors list
3. Type **Distance** (default: 100m)
4. Type **Resolution**
5. Type **Quadsegs** which controls the number of line segments to use to approximate a quarter circle when creating rounded offsets.
6. Select **Cap style** (default: round): controls how line endings are handled in the buffer.
7. Select **Join style** (default: round): Specifies whether round, miter or beveled joins should be used when offsetting corners in a line
8. Type **Mitre limit** (default: 5): Controls the maximum distance from the offset curve to use when creating a mitered join (only applicable for miter join styles). Minimum: 1.

.. image:: ../img/buffer_1.png
.. image:: ../img/buffer_2.png

Step 2: Click “Submit” button

Centroid
========

Creates a new point layer, with points representing the centroids of the geometries of the input layer.

Step 1: Type input:

1. Type **Name**
2. Select **Vector** from Vectors list

.. image:: ../img/centroid_1.png
    :align: center

Step 2: Click “Submit” button

Rectify
=======

A method that approximates the prediction pixels into polygons making decisions based on the whole prediction feature space

Step 1: Type input:

1. Type **Name**
2. Select **Vector** from Vectors list
3. Type **Resolution**

.. image:: ../img/rectify_1.png
    :align: center

Step 2: Click “Submit” button

Row detection
=============

Row detection is performed automatically for straight and curved rows. The detected rows are used in many applications.

Step 1: Type input

1. Type **Name**
2. Select **Vector** from Vectors list

.. image:: ../img/row_detection_1.png
    :align: center

Step 2: Click “Submit” button

Simplify
========

Simplifies the geometries in a line or polygon layer. It creates a new layer with the same features as the ones in the input layer, but with geometries containing a lower number of vertices.

Step 1: Type input

1. Type **Name**
2. Select **Vector** from Vectors list
3. Type **Tolerance** : if the distance between two nodes is smaller than the tolerance value, the segment will be simplified and vertices will be removed.

.. image:: ../img/simplify_1.png
    :align: center

Step 2: Click “Submit” button

Vector Clip
===========

This algorithm clips a vector layer using the features of an additional polygon layer. Only the parts of the features in the Input layer that fall within the polygons of the Overlay layer will be added to the resulting layer.

Step 1: Type input

1. Type **Name**
2. Select **Vector** from Vectors list
3. Select AOI from AOIs list

.. image:: ../img/vector_clip_1.png
    :align: center

Step 2: Click “Submit” button