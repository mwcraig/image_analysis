Multi-aperture photometry in AstroImageJ
=========================================

AstroImageJ, like other similar software packages, makes it easy to do photometry on several stars at once. 

Multi-aperture photometry is a little more interesting if there is more than one image to work on (but note, for the record, that you could do multi-aperture photometry on a *single* image, which might be useful for, say, a star cluster), so... 

+ Open all of the EY UMa images in a stack.
+ **MAKE VERY SURE YOU CHECK THE "Use virtual stack" BOX**. If you forget, ImageJ will complain, then quit.

+ Once you have the stack open, click the multi-aperture photometry tool: |multi-button|
+ In the box that opens, make sure you **uncheck** the "Use previous...apertures" option and **check** the "Use single step mode..." option. Ideally, set it up as shown here: |multi-setup|

Doing the photometry
---------------------

#. First, left-click on your target star.

    + There is nothing special about the target star except that ImageJ draws the rings around it in a different color, and handles it differently in the automatic graphing that it does.

#. Next, left-click on as many other stars as you want photometry for. For this exercise, select a total of three stars, including the target. The three stars you should look at are shown below:

|stars-to-look-at|

#. When you have selected all of the stars you want, **right-click** anywhere in the image. AstroImageJ **SHOULD NOT** start advancing through the stack, automatically finding the stars in each image. The only thing that may happen is many, many windows will open to begin graphing the magnitudes you measure. Find your way back to the image sequence window, which will have the circles on it for the stars you selected.

#. **Left-click** once, anywhere in the image. This will advance you to the next image in the sequence. Left-clicking once on the target star should overlay *all* of the apertures on the image. 

#. Left-click again to move to the next image, then left-click on the target star, and repeat until you get to the end of the sequence.

.. note::
    AstroImageJ has a mode in which it attempts to automatically locate the stars in images in the 
    sequence after the first, but you *should NOT use it* with v2.1.4. The new centroiding algorithm,
    which greatly improves reproducibility of AIJ magnitudes, is not a good match to the method currently
    used to identify the stars in images in the sequence.

#. Save the data table.

.. todo::

    #. Open the image "reference-positions.fit" to get the RA and Dec for each of the stars you look at and write them down in your notebook.

.. |multi-button| fancybox:: _static/multi-aperture-button.png
    :alt: Multi-aperture button
    :width: 5%
    :height: 5%

.. |multi-setup| fancybox:: _static/multi-aperture-setup.png
    :alt: Screenshot of multi-aperture setup
    :width: 5%
    :height: 5%

.. |stars-to-look-at| fancybox:: _static/stars-to-look-at.png
    :alt: EY UMa star field
