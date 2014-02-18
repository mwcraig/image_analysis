Basic Photometry in AstroImageJ
================================

+ Turn on the show-ring button (you must have an image open) |show_sky|

Initial guess for the aperture size
------------------------------------

#. Click line selection tool
#. Draw line across one of the stars that is circled in this image (or the image of interest to you:

|m34_sources|

#. Select `Analyze -> Plot seeing profile`
#. When asked whether to save the aperture radii, make the following changes:

    + Make the gap between the aperture radius and the inner sky radius at least 5 pixels
    + Make the difference between the inner and outer sky radii at least 10 pixels

.. note::
    
    This is **not** the best way to set the aperture size or the inner and outer sky radii. We will come back to how to best choose those later.

.. todo::

    #. What is the FWHM of the star you took the seeing profile of? 
    #. What does the FWHM mean? Answer both in terms of what the acronym means and an explanation in plain english what it represents. 
    #. What aperture size was chosen? How large is it compared to the FWHM (e.g. 2X, or half)?

Setting up aperture photometry
-------------------------------

#. Double click on the photometry tool in the toolbar. |photometry|
#. Check that the first window that opens matches this, except for the aperture radius and the inner and 
   outer sky radii, which you should choose based on the FWHM: |photometry_settings_1|
#. When done, click OK, and in the next window that opens check/set several things:

    * Gain for the Apogee Alta U9 is roughly 1.48 (feel free to use the value you got earlier this semester)
    * Read noise is roughly 28 or 29 electrons per pixel (feel free to use the value you got earlier)
    * Dark current is about 0.2 electrons per pixel per second
    * The Apogee Alta U9 saturates around 38000 counts.
    * Change the FITS headers output to list only AIRMASS and EXPOSURE as shown below, and make sure the boxes you have checked include *at least* all of the ones in the image below. |photometry_settings_2|
		
#. Click OK

Doing aperture Photometry
-------------------------

#. Choose one of the stars circled in red below, then, **IN IMAGEJ**, click on the star. |m34_sources|
#. Photometry information will appear in the measurement window.

.. todo::

    #. Write down, from the measurement table, for the star you chose:

        * the RA and Dec (in decimal hours and decimal degrees)
        * net counts (Source-Sky)
        * source radius
        * minimum and maximum sky radius
        * Sky counts/pixel
        * Source Error 
        * Source SNR

    #. What was the net number of photons received from the star in the aperture? Hint: Don't forget about the gain.
    #. Pay attention to the folks up front for a brief lecture about error and signal-to-noise ratio (SNR). Take useful notes.
    #. Calculate the source error and SNR and compare to the values of each from AstroImageJ
    #. What is the largest source of error? 
    #. Of the "noise" terms (dark, sky, read noise), which makes the largest contribution?
    #. How could you reduce that source of noise?


.. |m34_sources| fancybox:: _static/m34_comparisons.png
    :width: 50%
    :height: 50%

.. |photometry| fancybox:: _static/photometry_button.png
    :width: 20%
    :height: 20%

.. |show_sky| fancybox:: _static/sky_abackground.png
    :width: 10%
    :height: 10%

.. |photometry_settings_1| fancybox:: _static/photometry-parameters1.png
    :width: 5%
    :height: 10%

.. |photometry_settings_2| fancybox:: _static/photometry-parameters2.png
    :height: 5%
    :width: 5%


