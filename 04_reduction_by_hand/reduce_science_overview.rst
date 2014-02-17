Reduction of a science image: overview 
=======================================

Some Vocabulary
----------------

A *science* image is an image from which you hope to measure something; in other words it an image that is not a bias or a dark or a flat.

The term *reduction* means calibration of a an image to compensate for the effects of bias level, dark current and non-uniform illumination of the CCD.

We will make a distinction between a dark *frame*, which is the raw image that comes from the telescope when you ask it to shoot a dark, and a dark *current* image, which is a dark frame with the bias removed. This language isn't standard. Typically people simply use the word "dark" to refer to both even though they are different things.


Reduction: the concept
-----------------------

In practice this calibration takes two forms depending on the way you choose to compensate for the effects of dark current. In one form you compensate for dark current and bias in one step; in the other compensating for dark and bias is two separate steps.

Which way you go depends on the answer to one question: *Are your dark frames the same exposure time as your your science images?* 

If the answer is you have the option of compensating for dark current and bias in one step; if the answer is no you have to separate the steps.

Reduction steps 
----------------

Case 1: dark and science images have different exposure times
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

In an equation-like form image reduction looks like this:

.. math::

    \mathrm{science}_{reduced} = \frac{\mathrm{science}_{raw} - \mathrm{master~bias}-\mathrm{dark~current}_{scaled}}{\mathrm{master~flat}_{reduced,~normalized}}

Note there is a lot of work buried in here, much of which you have learned how to do in previous labs:

+ Create a master bias from your bias frames for the night.
+ Create a master dark **current** image by removing the bias from several dark **frames** and combining those bias-subtracted frames.
+ Scale the dark current image to match the science image exposure time.
+ Create a master flat by calibrating several flat images using the master bias and dark, normalizing the images and combining those to make a master image.

Once you have done all of those things, reducing the science image is straightforward. You use the image calculator in AstroImageJ to subtract bias and dark current from the raw science image, then divide by a *normalized* master flat.

.. todo::

    #. Suppose your dark *frames* were exposed for 30 seconds but your science images were 90 second exposures. Explain how you would need to adjust the dark *current* images to use them for removing dark current from your science image.

Case 2: dark and science images have the same exposure times
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

In an equation-like form image reduction looks like this:

.. math::

    \mathrm{science}_{reduced} = \frac{\mathrm{science}_{raw} - \mathrm{dark~frame}}{\mathrm{master~flat}_{reduced,~normalized}}

Note the difference between this case and the other: The dark *frame* includes both bias and dark *current* so we only need to do one subtraction from the raw science image.

.. todo::
    
    #. If for some reason you wanted to could you still, even in case 2, do the data reduction the way it is in case 1? Explain.

.. Notes to self
    Quick calib steps, once masters are in hand:

    + Load sequence
    + Use image arithmetic on sequence

    On EY UMa 060R note:

    + bright pixel at 1509, 1146 removed by dark
    + dust donut near 2951, 1364