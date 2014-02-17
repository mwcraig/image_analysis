Median or Average?
================================

Setup
-----

#. Please close any open images.
#. Open, as an image sequence, all of the files in the folder `images/funny_flats`

    * Remember, you need to open at least one FITS images before you have the option of opening a sequence!

.. todo::

    #. What is different about the first image in the sequence? Look near pixel coordinates `(1480, 820)`

Stacking, two ways
------------------

Stack all 10 of the images in two different ways:

* Average intensity
* Median

then answer these questions...

.. todo::

    #. Can you see the defect in the image made by averaging the stack? Why?
    #. Can you see the defect in the image made by median combining the stack? Why?
    #. In which stacked image is the defect more visible, the average or the median?

Median magic: The ideal case
----------------------------

Each of the flat images in your sequence has a somewhat different average value, presumably because the light source was fluctuating slightly in brightness. Furthermore, that variation is reasonably large (for this set of images the average pixel value ranges from about 22,900 to 23,300). The result is that the presence of the comic ray tends to bias the median towards slightly larger values at the position of the cosmic ray so that it is **is not** perfectly eliminated even when you median combine 10 frames.

For something like flat frames you really want to be combining images that have the same light level (within the limits of the read noise of the detector, anyway). Sometimes you can get that by having a very, very steady light level (a floodlight ought to deliver that, but doesn't). Sometimes that steady light level is nearly impossible (if you are shooting flats near twilight, for example).

Fortunately, there is a way to compensate by *normalizing* (or scaling) the images so that they all have the same typical value. `AstroImageJ` can do that normalization for you by following these steps:

* Open a sequence if you don't already have one open.
* Go to the menu `Process -> Normalize image/stack...`
* In the popup that opens you can set two options:

    * Whether to use mean or median as the "typical" pixel value (you almost always want median)
    * What you want the final value of the "typical" value to be after processing. 

.. warning::

    Normalizing will change the pixel values in the images you have open and there is no way to undo it. If you make a mistake you need to close the image stack and reopen it from the original files.

.. todo::

    #. If you haven't yet, normalize the sequence of flat images you have open. Is the average pixel value in the image roughly the same in each image after normalization? Why isn't the average pixel value the same as the median pixel value you set in the normalization dialogue box?
    #. Suppose one of the original images had a median pixel value of 23,200 and that you want to have want the median after normalization to be 2. Describe in detail what you need to do to the image to normalize (detail in the sense of the math operations you would need to carry out if you were to normalize by hand, not details of how to do it in `AstroImageJ`) and explain why your answer is correct.
