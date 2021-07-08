# Cog detector
This project is a gear teeth (cog) detector and counter using classic Computer Vision techniques with OpenCV.

## Images
The background of the input images is expected to be lighter than the object, just like in the example image:
![example](img_examples/example.png)

## Method
The image processing techniques applied to detect and count the cogs are the following:
1. Detect gear by segmenting the image.
2. Detect the inner circle by morphological opening region.
3. Obtain cog pixels by subtracting inner circle of the segmented image.
4. Detect cogs by finding connected components.

## Results
The result for the example image is: 35 cogs