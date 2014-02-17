Measurements in Astro ImageJ
============================

Selecting a region
------------------

In the AstroImageJ toolbar are a number of selection tools. They include the line selection tool, a rectangle selection tool, and several others.

* Start by selecting a rectangular region in one of your bias images.
* Now try selecting *exactly the same region* in a different bias image. Can you? Don't waste a lot of time trying please!

To take consistent measurements across a series of images it would be helpful to be able to tell AstroImageJ explicitly what region you want. You can do that by:

* Click on the toolbar so it is on top.
* Select `Specify` under the `Selection` menu under the `Edit` (i.e. `Edit -> Selection -> Specify`)
* You can set the size and position of the selection.

.. todo::
    
    #. Where is the origin used for the x and y position? In other words, where in the image is the point (0,0)?
    #. What is the position of the center of the image?

Taking a measurement
--------------------

Once you have selected a region you can measure a number of the properties of the pixels in that region. You can control which things are measured by going to one of two menus:

* Go to `Analyze -> Set Measurements...` if the AstroImageJ toolbar is on top, *or*...
* Go to `Edit -> Measurement Settings...` if an image window is on top.

To make a measurement, type Cmd-M, or select `Analyze -> Measure`.

.. note::

    Be sure that you are set up to measure at least the bounding rectangle, mean, median and standard deviation of the selected region.

.. todo::

    #. Measure the mean pixel value and the standard deviation of the pixel value for one of the images you have open.
    