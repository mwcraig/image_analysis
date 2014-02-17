Sequences of Images in Astro ImageJ
====================================

Before you begin
----------------

You cannot open a sequence of imgaes in AstroImageJ until you have opened at least one FITS file...so start by opening the first image for this lab.

.. note::

    FITS is a format for storing data in a way that any computer platform can read *if it has the right software installed*. It is very widey used in astronomy in part because you can store both the data itself and information about the data, called *meta-data*, in the file. The meta-data is stored in the FITS header and the data was the image itself.

.. warning::

    There are two very different sets of menus displayed in AstroImageJ depending on whether the toolbar or an image window are on top in the display.

Opening a sequence of images
----------------------------

The idea here is that you need to tell AstroImageJ two things:

* Which folder the images are in
* Which files from the folder you want to load into a sequence.


#. Make sure you have an image window on top.
#. From the file menu, select "Open image sequence in new window..."
#. **Choose the folder** containing the images you want to open in a stack.
#. To **choose the images** to put in the sequence you have a few options:
    
    * Use them all; just click OK in the window `Sequence Options`
    * Choose the starting and ending image by specifying the number of the starting image and the increment.
    * Enter a phrase or number that is in the name of all of the images that you want to open. Note that CaSe mAtTers; if the file name contains the word 'bias', for example, but you put 'Bias' in the box in `Sequence Options`, AstroImageJ will find no images.
    * Enter a more complex pattern that matches the names of the files you want to include.

.. warning::

    Opening more than a few dozen images in a sequence may bring your computer to a grinding halt because by default AstroImageJ loads them all into the computer's memory. If you select `Use virtual stack` you avoid that problem because AstroImageJ only reads in single images when it needs them. That slows down processing a bit, so for small numbers of images it is easier to *not* use a virtual stack.

Pattern matching examples
^^^^^^^^^^^^^^^^^^^^^^^^^

AstroImageJ allows you to enter fairly complex patterns to match file names. In those patterns some symbols have a special meaning:

* Use a period `.` represent any single character.
* Use an asterisk `*` to represent zero or more of whatever character came before it.
* Put characters in square brackets `[]` to represent any one of the characters in the brackets.

For example, the patter `.*` will always match all files because the period matches any character and the asterisk indicates zero or more of those characters.

The pattern `twi-.*bias.*` would match all files whose name starts with `twi-`, has zero or more characters, then the word `bias`, followed by zero or more characteres.

The pattern `flood-.*00[1-9]B_flt.fit` matches any files whose name starts with `flood-`, followed by any of the numbers 001 through 009, then `B_flt.fit`

.. todo::

    #. For each file name below explain why the name would or would not match the pattern `twi-.*bias.*`

        * Twi-bias.fit
        * twi-diffuser-flat-001bias.fit
        * twi-diffuser-flat-001bias_flt.fit
        * twi-diffuser-flat-001bIas.fit

    #. Look at the list of the files in the folder `for_gain`. For each of the items below come up with a pattern that matches the right files. Check your patterns by starting to open an image sequence in AstroImageJ, selecting the folder `for_gain`, entering the pattern in the right place, and verifying that the correct number of files matches.

        #. All bias images that have "twi" in the name (should be 11 files)
        #. The images in the R band (R is in the file name) that also have "flood" in the name and are number 001 through 003 (should be 3 files).
        #. The images in the I band with "flood" in the name (10 items)
        #. The images in the I band with "flood" in the name whose number is odd (001, 003, etc) (should be 5 images)
    



