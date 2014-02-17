Basic image statistics
======================

The rule of thumb to remember is that combining images reduces noise. For science images that is largely because combining images is equivalent to a longer exposure, which will have more light. For flat images the reasoning is similar; a flat image is, after all, just collecting light in a special configuration, so more light will mean better signal. 

For bias images (and to a large extent our dark images, which are largely bias) combining images reduces the random error introduced by the electronics that read out the CCD. The series of activities and questions below lead you through *what* changes as you look at combinations of bias images and ask you to think about *why* those changes occur.

Setup
------

* Open **one** of the bias images in the folder `for_gain`.
* Make a histogram of the image and choose, based on the histogram, a reasonable upper and lower limit. *Use this same upper and lower limit* for all of the rest of the histograms you make.
* Open a sequence in a new window that contains *all* of the bias images in the folder (they all have the word bias in the name).

Combining by averaging, and some basic patterns
-----------------------------------------------

.. todo::

    #. Make a histogram for a single bias image. Note the width of the bias histogram, which is twice the standard deviation, and the mean.
    #. Combine *four* of the bias images. Do this by:

        * clicking on sequence window so that it is on top
        * clickking on the AstroImageJ toolbar to make sure the correct menus are displayed
        * selecting `Z-Project` from the `Stacks` menu in the `Image` menu (i.e. `Image -> Stacks -> Z-Project`) **and**...
        * ...choosing appropriate values for the starting and ending image in the sequence, **and**...
        * ...choose *average* as the method of combining.
        * Be sure to **write down the name** of the combined image.

    #. Make a histogram of the combination of four bias images. Compare the *mean* and *standard deviation* of the distribution for the combined images with the same numbers for the single image.
    #. Repeat for 8 bias images; note the mean and standard deviation.
    #. Repeat again for all 16 bias images; note the mean and standard deviation.
    #. Describe in words:

        #. How the histogram changes as you increase the number of images in the stack.
        #. How the mean changes as you increase the number of images.
        #. How the standard deviation changes as you increase the number of images.

    #. For this type of error it can be shown that the amount of noise (i.e. the standard deviation) should be inversing proportional to the square root of the number of images. Does this seem to be true, at least roughly, for the histograms you just compared?

Different ways of combining: average vs median
----------------------------------------------

.. todo::

    #. Combine four images *using median to Z-project* the images, and make a histogram of the combined image.
    #. Combine 16 images *using median to Z-project* the images, and make a histogram of the combing image.
    #. Does the pattern you observed for the change in noise as you increase the number of images still hold for median combining?
    #. Compare the mean and standard deviation of these histograms with the corresponding mean and standard deviation from the images combined using the average. Which results in less noise, combing by average or combining by median?
    #. Why might you median combine images even though there is slightly less noise if you combine images by averaging?


