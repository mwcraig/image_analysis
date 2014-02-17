Calculating gain: step-by-step
================================

Setup
------

* To avoid confusion, please close all open image windows.
* Pick two bias images and open them in separate windows.
* Pick two flat images of the *same type* (flood or twi) and the *same filter* and  open them in separate windows.

Calculating gain
----------------

For the gain we will need to:

    * Select the same region in each image
    * Find the average pixel value in that region in each of the four images.
    * Calculate the difference between the two bias images
    * Calculate the difference between the two flat images
    * Find the standard deviation of the pixel values in the same region in each of the difference images.

Let's do that:

.. todo::
    
    #. Write down the names of the images you chose.
    #. Select a region and write down its width, height, and x and  y position.
    #. Find the average pixel value in that region in each image you have open. Write them down, clearly indiciating which measure goes with which image.
    #. Calculate the difference between the two bias images.
    #. Calculate the difference between the two flat images.
    #. Measure the standard deviation in the region you chose in each of the two difference images. Write the result down, clearly indicating which measurement goes with which difference image.
    #. Calculate the gain for the CCD using the formula in Howell's book.
    #. Calculate the read noise for the CCD using the formula in Howell's book.