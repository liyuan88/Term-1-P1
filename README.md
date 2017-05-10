# Term-1-P1
Udacity Project

I start with importing the necessary Python libraries (matplotlib, numpy, cv2, math) that will be used later. A test image is shown as follows and its dimension is printed out (540*960*3).



I then define the following functions that help to identify the lane lines.

-	Grayscale: returns an image to grayscale.
-	Canny: applies canny algorithm with low/high threshold parameters.
-	Gaussian_blur: applies Gaussian smoothing with kernel size.
-	Region_of_interest: applies an image mask that removes the parts outside the region of interest.
-	Draw_linear_regression_line/Draw_lines: Extrapolate the line segments to map out the full extent of the lane. The left/right lanes are separated by calculating the slope.
-	Hough_lines: applies hough transformation.
-	Weighted_img: combines the original image with the lane lines drawn by the model.


The process_image function combines the above functions and will be used in the video pipeline. I have tried some combinations of the parameters and the followings appear to give the best result.

 

The video output is attached as a separate document.
