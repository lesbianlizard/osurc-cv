The color-detect module is designed to find irregularities 
in image histograms, and on detection will pass the image 
to the next module in the funnel. 

Build/run instructions:

	make Basic-Histogram
	./Basic-Histogram

Algorithm: (in-progress)

-> create array for histogram Mats
-> fill array with histograms of incoming frames
-> compare incoming frames to histogram averages
-> if there are irregularities, pass img to next module

Portions of this algorithm can be replaced with an 
implementation of a background subtraction algorithm, such 
as MOG2. The background subtraction algorithm will need to 
be modified to account for histogram dimensions.

The next stage of the funnel is shape-recognition, 
followed by text-recognition. 
