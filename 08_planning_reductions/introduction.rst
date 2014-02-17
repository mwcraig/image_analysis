Introduction
============

+ We will assume you have gotten your science images through the initial calibration where you remove the biases, correct for dark current, and apply flat fielding corrections so that the illumination on the CCD is uniform.

+ Our goal for today is to help you decide just what you need to do to turn your initially calibrated science images into science.  This means:
	1. You need to figure out if you need to do more with the actual science images (e.g. stacking) to get the final images you will be working with.
	2. Assuming you will be performing photometric analysis of your images, i.e. measuring fluxes of your images, you need to figure out what, if any, photometric corrections you need to apply to your images.
	
+ **The Tools You Will Need:** In order to get your initially calibrated science images into science, you may need to use any or all of the following:
	+ ``AstroImageJ``, 
	+ ``JSkyCalc``,
	+  Microsoft Excel or some equivalent spreadsheet program,
	+ careful thought to plan out the reductions.

+ **BIG HINTS:** 
	+ Always take good notes describing what you are doing.  The level of detail should be such that someone else could reproduce your work based on your notes.
	+ Years of experience have shown us that we _will_ make mistakes ... many mistakes.  Its nothing personal, its just part of human nature.  However, you can prepare for making mistakes by always doing your analysis in such a way that you can back up and restart it if you discover an error.  The key to this is **NEVER OVERWRITE DATA FILES**!  When you are starting along a new analysis, image reduction, etc., always create new files, never overwrite old ones.  If you are introducing a new calculation to a spreadsheet, make a backup of the spreadsheet before you make extensive changes.  Always give yourself a way to recover from errors if you can. 

The Big Question 
-------------------

**Be ready to answer this question by ~12:15.**

.. todo::
    #. For my project to succeed, what do I need to actually accurately measure from my science images?
