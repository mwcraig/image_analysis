Choosing a Project
==================

+ Drs. Cabanela and Craig should have described the projects that are available to do.  As a reminder, here is a list of observing projects requiring new observations at the telescope:
	+ Variable Star observations (You will need to pick specific star).  It may be useful to use the `AAVSO Variable Star Plotter`_ to identify the star in the field.

		+ **EY UMa** has a period measured by Hollee Johnson; one more night of good data would be really helpful.
		+ **HR 7308** has an interesting history as the classical Cepheid with the shortest measured period (only 1.490808 days, measured by `Cabanela 1991`_) and one of only two known classical Cepheid variables whose amplitude of variability changes over time in a way that is not just "overtone beating" (the other Cepheid with this behavior is Polaris).  Cabanela has data from 20 years ago on this star, it would be interesting to see if this star is still varying with a period of 1.490808 days.  The only issue is the star is in Lyrae and not necessarily well positioned for Spring observations.
		+ **EL Dra** is listed as an RR Lyrae but has no reported period.
		+ **FK Peg** has no reported period; must be checked in the Catalina Sky Survey to see if data is available indicating that it is *not* variable.
		+ **EN Cep** has a partially measured light curve with data in the AAVSO database. Additional well-planned observations could refine the estimated period.
		+ **BU Cam** has a measured period, but a few well-planned nights could measure the period with much higher precision.
		
	+ Construction of a Color-Magnitude diagram (for example, V vs. V-R) for a globular or open star cluster.  Some possible candidates (not terribly well vetted) include:
		+ **NGC 1039 (Open Star Cluster)**: Fits on CCD frame, *have data on disk already.*
		+ **NGC 1912 (Open Star Cluster)**: Will barely fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 1960 (Open Star Cluster)**: Nice diffuse stellar distribution.
		+ **NGC 2099 (Open Star Cluster)**: Does not quite fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 2323 (Open Star Cluster)**: Will barely fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 4147 (Globular Cluster)**: Very small on sky, may be very hard to distringuish stars.
		+ **NGC 5024 (Globular Cluster)**:
		+ **NGC 5053 (Globular Cluster)**: Somewhat sparse so may be easier to distinguish stars.
		+ **NGC 5272 (Globular Cluster)**: Will barely fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 5466 (Globular Cluster)**: Somewhat sparse so may be easier to distinguish stars.
		+ **NGC 5904 (Globular Cluster)**: Does not quite fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 6205 (Globular Cluster)**: Does not quite fit on CCD frame, so may have trouble finding other stars in the field to use for photometric calibration.
		+ **NGC 6341 (Globular Cluster)**: Very dense cluster, may be hard to separate stars.

	+ Verify that the radial light profile of an elliptical galaxy exhibits a `de Vaucouleurs profile`_ (a special case of the `Sersic profile`_).  This would require you developing some techniques for analyzing the radial light profile of a galaxy.  Some ellipticals you may want to consider looking at:
		+ **NGC 2300**: This elliptical galaxy is in an interacting system, so its profile may be distorted.
		+ **NGC 2256**: Has a prominent foreground star on top of it.
		+ **NGC 2340**: In a group of galaxies.
		+ **UGC 3021**: Has some prominent foreground ojbects nearby.
		+ You can also use `"Criteria query" in SIMBAD`_ to find other candidates if you want.  **HINTS FOR SIMBAD SEARCH**: A good galaxy morphological type (SIMBAD calls it "mttype") to search for would be "E0" or "E1", so that the eliptical is viewed almost face on.  You probably want to find galaxies with a major axis ("dimmajor") between 10 and 20 arcminutes.  Use *jSkyCalc* to figure out a reasonable RA range for Spring (about same as the Local Sidereal Time at Feder in the Spring) and remember SIMBAD expects RA in searches like this to be in *decimal degrees*, not *hours*.  Remember that Dec<0 degrees will be far from Zenith and have limited time at low airmass.
	
	+ Verify that the radial light profile of the disk in a spiral galaxy exhibits an exponential profile (a special case of the `Sersic profile`_).  This would require you developing some techniques for analyzing the radial light profile of a galaxy. Some spirals you may want to consider looking at:
		+ **NGC 2336**: Smaller galaxy with prominent arms, but closer to face on than other galaxies.
		+ **UGC 2885**:	
		+ **NGC 2903**: This galaxy is large enough, but has prominent spiral arms which may distort the profile.
		+ **NGC 2403**: This galaxy has an "Active Galactic Nucleus" which may distort the profile in the center.
		+ **IC 342**: Faint disk, but should be manageable with Feder. 
		+ You can also use `"Criteria query" in SIMBAD`_ to find other candidates if you want.  **HINTS FOR SIMBAD SEARCH**: A good galaxy ("otype" is "G") would have morphological type ("mttype") to search for would be "S". You probably want to find galaxies with a major axis ("dimmajor") between 5 and 20 arcminutes.  Use *jSkyCalc* to figure out a reasonable RA range for Spring (about same as the Local Sidereal Time at Feder in the Spring) and remember SIMBAD expects RA in searches like this to be in *decimal degrees*, not *hours*.  Remember that Dec<0 degrees will be far from Zenith and have limited time at low airmass.
				
	+ Try to detect the transit of a known exoplanet.  This would require you to do some work to identify candidate exoplanets.  The `Exoplanet Transit Database`_ will produce a list of predicted transits for any date, given the latitude and longitude of our observatory.  
	
	+ Try to measure the light profile of an eclipsing binary system and use this to determine the orbital parameters for the two stars.  This would require you to research eclipsing binaries a bit and identifying a star with an upcoming eclipse.  You may find this list of `Eclipsing Binary Ephemerides`_ from the AAVSO useful.
		
	+ Measuring the variation in color and magnitude of a star with increasing airmass at the Feder observatory.  This would best be done using known Landolt standard stars with established fluxes.  See `Landolt 1992`_  and `Landolt 2009`_ .

+ There are also possible projects that would not require new observations, but rather analysis of existing data.  These might be good alternatives if the weather doesn't hold up this semester.  These "no new observations" required projects include:
	+ Creation of master frames for each night for which there is useful calibration data. And identification of nights for which some or all calibration data is missing.
	+ Check of stability of bias pattern and level over time and camera temperature.
	+ Cross check of dome flats, diffuser twilight flats and regular twilight flats.
	+ **HT Vul** (We already have a few nights of good data.  The period falls in an interesting timescale, about 0.15 days, long for a delta Scuti star, short for RR Lyrae, might be SX Phoenecius).
   	+ **EE Lyn** (hard, will require stacking before photometry, several nights).

.. _de Vaucouleurs profile: http://en.wikipedia.org/wiki/De_Vaucouleurs%27_law
.. _Sersic profile: http://en.wikipedia.org/wiki/Sersic%27s_law
.. _"Criteria query" in SIMBAD: http://simbad.cfa.harvard.edu/simbad/sim-fsam
.. _Eclipsing Binary Ephemerides: http://www.aavso.org/eclipsing-binary-ephemerides
.. _AAVSO Variable Star Plotter: http://www.aavso.org/vsp
.. _Cabanela 1991: http://adsabs.harvard.edu/cgi-bin/nph-data_query?bibcode=1991JAVSO..20...54C&link_type=ABSTRACT
.. _Landolt 1992: http://adsabs.harvard.edu/cgi-bin/nph-data_query?bibcode=1992AJ....104..340L&link_type=ABSTRACT
.. _Landolt 2009: http://adsabs.harvard.edu/cgi-bin/nph-data_query?bibcode=2009AJ....137.4186L&link_type=ABSTRACT
.. _Exoplanet Transit Database: http://var2.astro.cz/ETD/predictions.php

.. todo::

	#. What project do you think you would like to attempt?
	