# codingdv
# Code written in Python 
# Assignment desciption below

Coding #2. Due Thursday 11/12/2020.
Spatial resolution.
C#2. A telescope has a theoretical spatial resolution q ~ l/D,
where q is the angular resolution (radians) in the image, l is the wavelength of light, and D is the
diameter of a telescope (or the maximum baseline for an interferometer array of telescopes). In this
coding exercise we will investigate the one dimensional brightness profile of two stars, as a function of
separation between the stars.
A. First we will model the spatial profile of an unresolved source (point source) using a Gaussian
function. Namely if the array variable “profile” has Gaussian shape then FWHM =2.*1.18*sigma where
profile = V*exp(-0.5*(x-xp)^2/sigma^2)
V is the peak brightness value
x is an array with 120 values ranging from 0 to 12 arcseconds
 x=0.0 + 0.1*findgen(120)
xp is the central position of the star
sigma is the standard deviation (assume sigma = 1.5 arcseconds)
FWHM stands for the Full Width at Half Maximum
Print,x ;will print out the values of x
resplot = Plot(x,profile ) ;will make a plot of the profile
resplot.save, 'resplot.jpg' ;will save the plot in jpg format
B. generate the brightness profiles of two stars
Profile1: V1 = 1.0 xp1= 3.0
Profile2: V2 = 1.0 xp2= 7.0
Make a plot of profile1 versus x, profile 2 versus x, profile sum of 1&2 versus x, on the same plot.
C. Change xp2, remake the plots, and describe how the profile sum changes for different values of
separation. At what separation (xp2-xp1) does the combined profile only have one peak value, rather
than two peak values? This is the minimum spatial resolution to distinguish two “point sources”, for
which it is no longer possible to tell whether there are one or two sources present. Compare your result
with sigma and also with the FWHM.
