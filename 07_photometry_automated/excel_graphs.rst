Magnitude and airmass
======================

**Please begin by opening your data table in Excel.**

Calculating instrumental magnitude
------------------------------------

BGO give a formula for instrumental magnitude in terms of counts:

.. math::

    m = -2.5\log_{10}(N_\text{Source}-N_\text{Sky}) +2.5\log_{10}(t) + C

where *t* is the exposure time, *N* is the number of counts and *C* is a constant that depends on filter and the CCD.

.. todo::

    #. Add three columns to your data table, one for the instrumental magnitudes of each of the three stars for which you have photometry. NOTE: AstroImageJ calls the columns that contain the net counts (i.e. :math:`N_\text{Source}-N_\text{Sky}`) something like `Source-Sky_T1` or `Source-Sky_T2`. Use a value of *zero* for *C*.


Airmass and instrumental magnitude
------------------------------------

In the last class we discussed extinction (also in Chapter 7 of BGO). In this part of the lab you will investigate the relationship  between airmass and instrumental magnitude.

In BGO the relationship  between the two is written

.. math::

    m = m_0 + k X,

where *m* is the instrumental magnitude, *X* is the airmass, and *k* is the extinction coefficient.

.. todo::

    #. Make a graph with airmass on the horizontal axis and instrumental magnitude on the vertical axis, like BGO Fig. 7.4. Use the "target" star.

        + Display the points as *points* not a line like the book does.
        + Excel will pick stupid default values for the airmass values; be sure to at least change the minimum value to something sensible.
    
    #. Add a trendline to each of the data series. In the options for the trend line:

        + Display the fit equation 
        + Display :math:`R^2`

    #. What would the instrumental magnitude of this star be if corrected for the atmosphere? *Hint*: What does :math:`m_0` represent, physically (mathematically it is the y-intercept of the line you fit to the data)


Airmass and color
------------------

According to BGO, stars of different color experience different extinction; this is shown in Fig. 7.6.

.. warning::

    Fig. 7.3(b) is **not** showing the way extinction changes for stars of different colors.

.. todo::

      #. Add the instrumental magnitudes of the other two stars to your graph. The graph should have three sets of points on it, one set for each of the three stars (i.e. three data series, in Excel-speak).
      #. Add trendlines to the new data series.
      #. Do all three stars experience the same extinction coefficient, *k*? Why do you think that is?