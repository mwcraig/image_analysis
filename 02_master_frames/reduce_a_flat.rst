Your first image reduction
===========================

As your very first experience with reducing (i.e. calibrating) an image you will calibrate one flat frame from the folder ``float``.

Open any one of the flat images whose name begins ``twi`` and is in the R filter (these have ``R`` in the name).

.. todo::
    
    #. Double-check the exposure time of the flat you opened. Does it match the exposure time of the master dark you created?
    #. Use the image calculator to subtract your master dark from the flat frame that you opened.
    #. In principle, the pixel values are now all due to light that fell on the CCD. Pick a pixel, and convert the value from ADU to photons using the gain you calculated earlier. How many photons was it?