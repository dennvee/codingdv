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


Instructions for running code 
Intructions 
In order to run this code python 3.0 is needed 

Resources for beginning with Python
Below is a link for downloading Python and very useful IDE's provided by Anaconda Navigator.
Anaconda navigator is a distribution package which included Python, IDEs and libraries. 
(simplifies the process substancially.None of the libraries used within my code need to be 
downloaded seperately as the distribution package includes all of this and more). 

link
https://www.anaconda.com/products/individual 
Once you are on the website scroll all the way to the bottom page and install Anaconda (options for Mac, PC, and Linux)

Once the Anaconda navigator is downloaded, launch the Aanaconda navigator. (should be found on mac using spotlight search)
Once the anaconda navigator is opened, click the home tab (on left side)
Then scroll until you see jupyter notebook and click launch. (Jupyter notebook is a user friendly 
enviornment for implementing this code)
Jupyter notebook will then request a desired path to be opened (I use google chrome). 
Once Jupyter notebook is opened, on the top right hand side, click the drop down 'New'>click
'Python 3'. Now you are ready to start coding! 

The other document titled 'Kepler_code_jupyter' provides the code used to 
complete the assignment, viewed through jupyternotebook. 

Alternatively! 
If you are familiar with python and wish to use your own editor, 
the code can be accessed through the document titled 'CPKeplerCode_'




