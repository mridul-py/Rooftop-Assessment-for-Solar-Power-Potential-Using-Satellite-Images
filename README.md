Rooftop Solar Power Potential Assessment Using Satellite Images
Overview
This project leverages AI-based technologies to assess the solar power potential of rooftops using satellite images. Given the lower resolution of satellite imagery in India compared to the US, we employ a variety of advanced image processing techniques to accurately identify and segment rooftop boundaries.



Features
Aerial Rooftop Detection
Hough Transforms
Watershed Segmentation
Adaptive Canny Edge Detection
Foreground and Background Separation
Gabor Filter
Building Rooftop Extraction
Edge Sharpening
Active Contours
Rooftop Polygon Approximation
Pixel-based Polygon Filling
Region-based Polygon Filling
Conversion from Google Maps to Image Pixels
Optimal Solar Panel Area Identification
Getting Started
Installation
First, install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Usage
Edge Extraction
Auto-Canny Edge Detection:
auto_canny.py
Edge Sharpening:
edge_sharpen.py
Watershed Segmentation:
watershed_pyrMeanShift.py
Foreground Background Separation
Gabor Filter:
gabor_test.py
Building Rooftop Extraction
Active Contours:
active_contours.py
Polygon Approximation
Pixel-wise Polygon Filling:
poly_fill.py
Region-based Polygon Filling:
polygon_fit.py
Conversion from Google Maps to Image Pixels
Latitude and Longitude to Pixel Conversion:
lat_long_metre_pixel.py
Optimal Solar Panel Placement
Combining Features for Optimal Area:
canny_corner.py
canny_contours.py
Final Solar Panel Placement:
panels_atlast.py
Methodologies
Aerial Rooftop Detection
Hough Transform
Description: Used for shape localization, primarily squares and rectangles. Limited effectiveness for non-rectangular shapes.
Adaptive Canny Edge Detection
Description: Effective edge detection on low-quality images but challenging for densely populated areas.
Watershed Segmentation
Description: Useful for counting buildings and plotting rooftop areas but fails in densely populated regions.
Gabor Filter
Description: Separates foreground (rooftops) from the background using frequency content analysis and Gaussian Mixture Models.


Building Extraction Methods
Edge Sharpening
Description: Enhances image quality to better mark rooftop edges.
Active Contours
Description: Optimizes rooftop area extraction using edge-based and region-based segmentation.


Polygon Approximation
Hough Transform
Description: Analyzes rooftop shapes and reduces Hough lines using K-Means clustering.
Pixel-wise Polygon Filling
Description: Marks rooftop areas by moving around the contour in a clockwise direction.
Region-based Polygon Filling
Description: Divides the rooftop area into regions and marks them based on intensity.


Conversion from Google Maps to Image Pixels
Description: Converts pixel values to square meter areas using the latitude and longitude of the region.
Optimal Rooftop Area for Solar Panels
Description: Combines Canny Edge Detection and contour analysis to identify the best areas for solar panel placement.


Conclusion
This project provides a robust set of tools and methodologies to accurately assess rooftop solar potential using satellite images. Despite the challenges posed by lower resolution images, the techniques implemented here offer reliable solutions for rooftop identification and optimal solar panel placement.
