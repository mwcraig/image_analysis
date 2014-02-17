From counts to magnitudes
==========================

Recall that magnitudes are fundamentally defined in terms of flux ratios:

.. math::
    m_1 - m_2 = -2.5\log\frac{f_1}{f_2}

We can't, strictly speaking, calculate the flux from an image because flux measures *energy* but a CCD just counts photons. One reason for using filters is that it at least restricts the photons that hit the detector to a narrower energy range than without a filter, so that the number of photons received is at least roughly proportional to the amount of energy received.

Setting aside the energy, the flux is the ratio of the counts from the star to the exposure time (really flux has units energy/time/area, but since we are using the same area for all of the stars we measure and we already agreed to punt on the energy, we are left with counts per time).

Instrumental magnitude
-----------------------

Though we can't actually calculate any magnitudes by themselves, ever, only magnitude differences, it is sometimes convenient to define an instrumental magnitude like this:

.. math::

    m_{inst} = -2.5\log(N/t) + C

where *t* is the exposure time, *N* is the number of total number of photons from the source (don't forget the gain!), and *C* is a completely arbitrary constant. You can choose any value you want as long as you consistently use that value for calculating all of your instrumental magnitudes.

.. todo::

    #. If you choose :math:`C=0`, what is the instrumental magnitude for the star you measured?
    #. Look at the table of magnitudes handed out (also `available here`_). Does your instrumental magnitude match the V magnitude of the star you chose? Should it?
    #. What would you have to choose *C* to be for your magnitude to match the magnitude in the table?

Magnitude differences
----------------------

Though instrumental magnitudes are not, by themselves, expected to match the magnitude in a catalog you might expect magnitude differences to match. Consider two stars whose instrumental magnitudes are :math:`m_{1,i}` and :math:`m_{2,i}`. Then the difference of the instrumental magnitudes is

.. math::

    m_{1,i} - m_{2,i} = \left(-2.5\log(N_1/t_1) + C\right) - \left(-2.5\log(N_2/t_2) + C\right)
                = -2.5 \log\left(\frac{N_1}{t_1}\frac{t_2}{N_2}\right)

If the exposure time is the same in both measurements, this simplifies a little bit, to

.. math::

    m_{1,i} - m_{2,i} = -2.5 \log\frac{N_1}{N_2}.

Since the constant *C* cancels out when we take a magnitude difference, we should expect that different observers will agree on magnitude *differences* even if the two observers use different instruments, different aperture sizes, and different exposure times. 

.. todo::

    #. Talk to someone who chose a different star than you did and calculate the difference in instrumental magnitude between your two stars.
    #. Compare your difference in instrumental magnitude to the difference in the reported magnitudes of the two stars in the table. 
    #. Try looking up your two stars in simbad and write down their V magnitudes according to simbad.

        * do a coordinate search
        * one format for entering coordinates is like: 2.703738h+42.77795d 
        * RA is first, in decimal hours, followed by declination in decimal degrees

    #. Does the magnitude difference as calculated from simbad match what you get from the table we provided? Does it match your image?


.. _available here: _static/mag_table.pdf
