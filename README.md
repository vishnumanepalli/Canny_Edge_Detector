# Canny_Edge_Detector

Aim:  

 To get hands-on experience implementing a very popular segmentation algorithm 

Introduction 

The  purpose  of  edge  detection  in  general  is  to  significantly  reduce  the  amount  of  data  in  an  image, 
while  preserving  the  structural  properties  to  be  used  for  further  image  processing.  Several  algorithms 
exists,  and  this  lab  focuses  on  a  particular  one  developed  by  John  F.  Canny  (JFC)  in  1986 .  Even 
though it is quite old, it has become one of the standard edge detection methods and it is still used in 
research  .  The  aim  of  JFC  was  to  develop  an  algorithm  that  is  optimal  with  regards  to  the 
following criteria: 

 Detection: The probability of detecting real edge points should be maximized while the 
probability of falsely detecting non-edge points should be minimized. This corresponds to 
maximizing the signal-to-noise ratio.  

 Localization: The detected edges should be as close as possible to the real edges.  

 Number of responses: One real edge should not result in more than one detected edge (one 
can argue that this is implicitly included in the first requirement).

The Canny Edge Detection Algorithm (Canny) 
 
The algorithm runs in 5 separate steps:

1. Smoothing: Blurring of the image to remove noise.  

2. Finding  gradients:  The  edges  should  be  marked  where  the  gradients  of  the  image  has  large 
magnitudes. 

3. Non-maximum suppression: Only local maxima should be marked as edges. 
 
4. Double thresholding: Potential edges are determined by thresholding. 

5. Edge  tracking  by  hysteresis:  Final  edges  are  determined  by  suppressing  all  edges  that  are  not 
connected to a very certain (strong) edge.
