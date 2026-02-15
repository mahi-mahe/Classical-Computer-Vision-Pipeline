# Classical-Computer-Vision-Pipeline
A beginning tour to computer vision pipeline from image acquisition, preprocessing, segmentation, feature extraction, feature matching, recognition and final output.
# Classical Computer Vision Pipeline using OpenCV

This project demonstrates a step-by-step classical computer vision workflow using OpenCV.  
It follows the traditional approach from image capture to feature analysis, matching, and simple decision making.

---

## Pipeline Overview

The system processes visual data through the following stages:

1. **Image Acquisition** – capture from webcam or load from file  
2. **Pre-processing** – grayscale conversion, noise reduction, contrast enhancement  
3. **Segmentation / ROI** – thresholding and contour extraction  
4. **Feature Extraction** – ORB keypoints and descriptors  
5. **Feature Matching** – Brute Force matching with Hamming distance  
6. **Classification** – simple rule-based labeling using contour area  
7. **Post-processing** – Non-Maximum Suppression (NMS)

An additional example shows classical **Haar Cascade** detection for faces and eyes.

---

## Methods Used

- Gaussian Blur  
- Histogram Equalization  
- Binary Thresholding  
- Contour Detection  
- ORB (Oriented FAST + BRIEF)  
- BFMatcher  
- NMS (Non-Maximum Suppression)  
- Haar Cascade classifiers  

---

## How to Run

Each step is written as an independent block.  
Provide required input images (e.g., `acquired_image.jpg`, `another_image.jpg`) and run sequentially.

Webcam can be replaced with:

```python
frame = cv2.imread("image.jpg")
