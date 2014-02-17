Master frames
=============

Overview
--------

Master frame is a combination (stack) of calibration frames of the same type. The preferred method of combination is median, to eliminate artifacts like cosmic rays, unless you have some good reason for averaging instead.

.. note::
    For this part use the images the folder from the last lab (called `float`).

Master Bias
------------

.. todo::

    #. Make a master bias frame using all of the bias frames in the folder and save the result as a FITS image. Make a note of:

        * Which files went into the master.
        * How you combined the files.
        * How many files went into the master.
        * What you called the master bias frame.

.. note::
    When you are done making the master bias, you can close the image sequence. 

Master Dark 
-----------

There are two different ways the term master dark is used; in some ways that is because there are two contributions to the  counts in a dark frame:

    Dark counts = bias + thermal electrons (aka dark current)

One version of a master dark contains **all** of the dark counts, including the bias. The other includes **only** the contribution from the thermal electrons.

The first variety is convenient because you can use that single master to remove both bias and thermal electrons from your images. The second variety is necessary if some of the science images you have do not have the same exposure as your dark frames because the second variety can be scaled to different exposure times.

Today we will focus on the first variety, master darks that also include the bias.

Dark frames of different exposure time *should* have different pixel values...which means you should only combine dark frames *that have the same exposure*.


.. todo::

    #. Make a master dark. Use all of the files in the `float` folder that start with ``twi`` and have ``D15`` in the name. Combine using a median, and save the result as a FITS image. Make a note of:

        * Which files went into the master.
        * How you combined the files.
        * What the exposure time was for these darks.
        * What you called the master dark frame.

.. note::
    When you are done creating the master dark you can close the image sequence of darks.
    
Master Flat
-----------

Remember that a flat really is an image of something: uniform illumination. Just like an image of something more interesting (like stars), it needs some basic calibration before it can be used to correct for differences in illumination in science images.

We will return to the procedure for finding a master flat in a little bit, after walking through the most basic parts of image reduction.

