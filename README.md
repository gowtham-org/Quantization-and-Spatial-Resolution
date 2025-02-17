# Quantization-and-Spatial-Resolution

 Image Processing: Intensity-Level Quantization and Spatial Resolution Reduction
This project demonstrates two fundamental image processing techniques:
Intensity-Level Quantization: Reducing the number of intensity levels in a grayscale image.
Spatial Resolution Reduction: Reducing the spatial resolution of a grayscale image.
The project includes Python implementations, visual results, performance analysis, and graphs to analyze the effects of different parameters.

Table of Contents  
##Introduction  
##Implementation Details  
###Intensity-Level Quantization  
###Spatial Resolution Reduction  
##Visual Results and Analysis  
##Performance Analysis  
##How to Run the Code  
##Dependencies  
##Conclusion  

Introduction
Image processing techniques like quantization and resolution reduction are essential for tasks such as image compression, optimization, and analysis. This project explores:
Intensity-Level Quantization: Reducing the number of intensity levels in an image to achieve compression or artistic effects.
Spatial Resolution Reduction: Reducing the number of pixels in an image to decrease its spatial resolution.
The project includes:
Python implementations of both techniques.
Visual results for different parameter values.
Performance analysis (execution time vs. parameter values).

Implementation Details
Intensity-Level Quantization
Objective: Reduce the number of intensity levels in a grayscale image.
Parameters:
bit_depth: Number of bits used to represent intensity levels (1–8)
Output: Quantized images for different bit depths.
Spatial Resolution Reduction
Objective: Reduce the spatial resolution of a grayscale image.
Parameters:
factor: Reduction factor (e.g., 2, 4, 8).
Method:
The image is resized using cv2.resize() with INTER_AREA interpolation.
Output: Reduced-resolution images for different reduction factors.

Visual Results and Analysis
Intensity-Level Quantization
Low Bit Depth (1-bit):
Results in a binary image with only two intensity levels (black and white).
Fine details are lost, and the image appears pixelated.
Medium Bit Depth (2-bit, 4-bit):
Preserves some details but introduces visible banding artifacts.
High Bit Depth (6-bit):
Produces images close to the original quality with minimal banding.
Spatial Resolution Reduction
Low Reduction Factor (2x):
Slightly reduces image size while preserving most details.
Medium Reduction Factor (4x):
Reduces image size noticeably, with some loss of details.
High Reduction Factor (8x):
Significantly reduces image size, resulting in a blocky appearance.

Performance Analysis
Intensity-Level Quantization:
Execution time is consistent across different bit depths.
The quantization process is computationally lightweight.
Spatial Resolution Reduction:
Execution time increases slightly with higher reduction factors.
Larger reduction factors result in smaller images, which are faster to process.
Graphs
Quantization: Execution Time vs. Bit Depth
Flat line, indicating consistent execution time across bit depths.
Resolution Reduction: Execution Time vs. Reduction Factor
Slight increase in execution time as the reduction factor increases.

How to Run the Code
Steps
Clone the repository or download the Python scripts.
Place your images in the specified directory and update the image_paths variable in the script.
View the visual results and performance graphs.
 
Dependencies
Python 3.x
Libraries:
opencv-python-headless
numpy
matplotlib
Conclusion
This project demonstrates the effects of intensity-level quantization and spatial resolution reduction on grayscale images. Key takeaways:
Quantization: Bit depth controls the trade-off between image quality and file size.
Resolution Reduction: Reduction factor controls the trade-off between image size and detail preservation.
Both techniques are useful for image compression and optimization, with applications in computer vision, multimedia, and data storage.
 

