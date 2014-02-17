Calculating gain
=================

Please take a look in Howell, pages 71-73, for a description of how to calculate gain and read noise from bias and flat images. The relevant equations are also on the board at the front of the room.

Note that to calculate the gain and read noise there are a few things we need to be able to do:

    * Select a region of an image that doesn't include the edges, because Howell suggests that the pixels at the edges tend to be more problematic, and these images may have an overscan region.
    * Calculate the average value of the pixels in that region.
    * Calculate the difference between two images (i.e. the result of subtracting one image from the other).
    * Find the standard deviation of pixels in that difference image in the same region selected orginally.

In principle, none of these things are hard. In practice it also isn't that hard...once you know how to do it. For that we'll take a detour into how to use AstroImageJ.
