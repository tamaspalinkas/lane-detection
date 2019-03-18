# Lane detection from video
Python implementation of lane detection optimized for own dashcam video.

# Description
The image processing pipeline consist of converting the image to grayscale, applying Canny edge detection over a triangle shaped area of interest, then applying Hough transform to extract lines.

The grouping of the left and right lanes are done by finding the extracted lines with extreme slopes. Fitting lines to the groups represent the lanes on the output video.

The implementation performs well on highway footage as it is capable of the detection of straight lines, and it needs further extension to funcition under different road conditions.

# Details

### Libraries
- opencv
- moviepy

# Demo
<img src="https://github.com/tamaspalinkas/lane-detection/blob/master/lane-detection.gif">
