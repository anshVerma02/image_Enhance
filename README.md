
# Image Enhancement and Analysis Pipeline
This project is an image enhancement and analysis pipeline designed to improve visual quality and analyze key characteristics of images using OpenCV, NumPy, and skimage libraries. The project is developed in Google Colab and is intended to be a useful tool for enhancing images and understanding their properties through entropy analysis, histogram comparison, superpixel segmentation, and distance mapping.


## Features

- ***Color Correction:*** Adjusts color distribution using LAB color space to improve overall balance.
- ***White Balance:*** Balances color tones to correct color casts.
- ***Contrast Enhancement (CLAHE):*** Applies Contrast Limited Adaptive Histogram Equalization to enhance image contrast.
- ***Superpixel Segmentation:*** Segment images into superpixels using the SLIC algorithm.
- ***True Distance Mapping:*** Estimates distance based on brightness in LAB color space.
- ***Comprehensive Visualization:*** Includes entropy, histogram, and RGB channel comparison for each step.


## Project Overview
The pipeline takes an input image and applies a series of enhancement techniques in the following order:

- Color Correction
- White Balance
- Contrast Enhancement using CLAHE
Each enhancement step is accompanied by visualizations to help understand the impact on entropy, histograms, and pixel distributions. Additionally, superpixel segmentation and true distance mapping are performed for further image analysis.


## Getting Started
### Prerequisites
- ***Google Colab:*** The project is designed to run in Google Colab.
- ***Python Libraries:*** OpenCV, NumPy, Matplotlib, and skimage.
## Installation
This project can be run on Google Colab to ensure easy access to necessary libraries and GPU acceleration, if available. Follow these steps to set up and execute the project:

### Clone the Repository:
- Open Google Colab.
- Run the following command to clone the repository into your Colab environment:

```bash
!git clone https://github.com/anshVerma02/image_Enhance.git
%cd image_Enhance


```
#### Install Required Libraries:
- The following libraries are required: ***opencv-python, numpy, matplotlib, scikit-image***. 
- Run the following cell in Colab to install any missing dependencies:

```bash
!pip install opencv-python-headless numpy matplotlib scikit-image

```

#### Upload an Image:
- The project includes an interactive upload step to process a custom image. Use the upload cell within the Colab notebook to upload an image directly.

#### Run the Notebook:
- After cloning and installing dependencies, run each cell in sequence to perform color correction, white balancing, CLAHE enhancement, entropy analysis, and visualization of the image processing steps.
- Outputs like entropy values, histogram comparisons, superpixel segmentation, and true distance estimation will be displayed as plots within the Colab notebook.


## Code Walkthrough
1. Load Image
- The user uploads an image, and the pipeline reads it as the input image.
2. Color Correction
- Enhances color distribution in the image using the LAB color space to balance colors.
3. White Balance
- Adjusts image color tones for a more natural look.
4. Contrast Enhancement (CLAHE)
- Uses CLAHE to enhance the contrast, especially for low-contrast images.
5. Visualization and Analysis
- Each processing step is visualized with:
  - *RGB Histograms:* Comparison of pixel intensities across RGB channels.
   - *Entropy Plot:* Shows the entropy values to indicate the level of information and contrast.
   - *Grayscale Histograms:* Comparison of pixel distribution across grayscale intensities.
6. Superpixel Segmentation
- Segments the image into superpixels using the SLIC algorithm.
7. True Distance Map
- Uses the brightness channel in LAB space to generate a distance map estimation.
8. Final Comparison
- Displays a side-by-side comparison of the original image vs. the fully enhanced image.
## Visualization Examples
- ***RGB Channel Histograms:*** Shows pixel distributions for each color channel (R, G, B).
- ***Entropy Comparison:*** Plots entropy at each step to visualize information gain or loss.
- ***Superpixel Segmentation:*** Displays segmented superpixel regions.
- ***True Distance Map:*** Visualizes estimated distances based on brightness.
## Results
The final output is an enhanced image that has gone through color correction, white balancing, and contrast enhancement, along with detailed comparisons and metrics at each step.
## Authors / Contributors

- [@anshVerma](https://www.github.com/anshVerma02)
- [@smriti]()
- [@swayam]()
- This project was developed collaboratively. Feel free to contribute or fork the repository for your own applications.


## License
This project is open-source and licensed under the MIT License.
