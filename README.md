# regionprops3
regionprops3 measures the geometric properties of image objects in 3D space.

Objects are defined as connected pixels in 3D. This function 
uses regionprops to get pixellist from the binary image. If you'd like
to define objects connectivity on our own, use bwlabeln first. 

output = regionprops3(img,properties) takes 3-D binary image or output 
from bwlabeln and returns measurement as specified by properties. If no
property is specified, the function will return all measurements by 
default.

output = regionprops3(img,'IsPixList', properties) takes an M x 3 matrix of
pixel list as input and returns measurements. 

Properties can be a comma-separated list of strings such as: 

'MajorAxis' : returns a unit vector that points in the
direction of the major axis

'MajorAxisLength' : returns the length of the major axis

'Centroid' : returns the centroid of the object

'AllAxes' : returns measurements of all three principal axes of image
objects, including axis directions, eigenvalues and axis lengths, all
organized in descending axis length. 

'Eccentricity' : returns Meriodional Eccentricity, defineds as the 
eccentricity of the section through the longest and the shortest axes
and Equatorial Eccentricity, defined as the eccentricity of the 
section through the second longest and the shortest axes. 

Version 1.1.1
Copyright 2014 Chaoyuan Yeh
