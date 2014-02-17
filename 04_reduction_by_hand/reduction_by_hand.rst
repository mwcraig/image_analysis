Science image reduction
========================

Look at the images in the folder ``reduce-by-hand``. It contains a master bias frame a couple of master dark frames (these have *not* had the bias subtracted from them), a master flat, and a science image.

.. todo::

    #. Examine the FITS headers of the images. Which of the two data reduction cases in the previous discussion applies here? Explain.
    #. Reduce the science image.

        #. First, subtract of the bias/dark current or the dark frame (depending on which case applies here). Identify one or more features of the image that visibly changed when you did this step of the calibration.
        #. Second, use the flat field to correct the illumination. Describe what changes, if any you see in the image. *Hint:* As with the previous step, you will need to use the image calculator.

    #. Summarize, in your own words, the steps needed to reduce a science image.