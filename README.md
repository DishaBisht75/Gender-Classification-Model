# Gender-Classification-Model

A machine learning project that classifies gender from facial images using image processing and statistical feature extraction. The model extracts features from images in the HSV color space and uses a Support Vector Machine (SVM) classifier for prediction.

PROJECT OVERVIEW

This project builds a gender classification system using traditional machine learning techniques. Instead of deep learning, it focuses on feature engineering and statistical analysis of images.
Images are preprocessed, converted into HSV color space, and multiple statistical features are extracted from each channel. Additional binary image features and edge-based features are also used to improve classification performance.

FEATURES

1. Image preprocessing using OpenCV
2. Conversion of images to HSV color space
3. Statistical feature extraction from H, S, and V channels:
   1. Mean
   2. Standard deviation
   3. Skewness
   4. Kurtosis
   5. Entropy
   6. Median
   7. Intensity range
5. Binary image generation using Otsu Thresholding
6. Edge detection using Canny Edge Detector
7. Additional structural features:
   1. White pixel ratio
   2. Black pixel ratio
   3. Edge density
8. Feature scaling using StandardScaler
9. Classification using Support Vector Machine (SVM) with RBF kernel

TECHNOLOGY USED
1. Python
2. OpenCV
3. NumPy
4. SciPy
5. Scikit-learn
6. Matplotlib

PROJECT WORKFLOW

1. Load male and female image datasets.
2. Resize images to 100 × 100 pixels.
3. Convert images from BGR to HSV color space.
4. Extract statistical features from the H, S, and V channels.
5. Generate binary images using Otsu thresholding.
6. Extract structural features such as pixel ratios and edge density.
7. Normalize features using StandardScaler.
8. Train an SVM classifier.
9. Predict gender for new images.

MODEL OUTPUT

The trained model predicts the gender label along with a confidence score.

Example:

image1.jpg → Male (91.4% confidence)

image2.jpg → Female (87.6% confidence)

DATASET STRUCTURE

dataset/
   male1/
   female1/

test/
   test_images/
   
HOW TO RUN

1. Clone the repository

git clone https://github.com/yourusername/gender-classification-ml.git

2. Install required libraries

pip install numpy opencv-python scikit-learn scipy matplotlib

3. Run the training notebook or script.

FUTURE IMPROVEMENTS

1. Use CNN / Deep Learning models for higher accuracy
2. Increase dataset size
3. Add real-time webcam gender detection
