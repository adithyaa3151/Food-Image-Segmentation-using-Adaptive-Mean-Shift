# Food Image Segmentation using Adaptive Mean Shift

This project applies **image segmentation** techniques for food image processing using an **adaptive Mean Shift clustering algorithm**. The approach enhances segmentation accuracy by **applying color transformations, contrast stretching, and morphological filtering**, achieving a **high Mean Intersection over Union (mIoU) score of 0.9501**.

## Project Overview
This project explores **food image segmentation** using the **Mean Shift clustering algorithm**. The approach integrates **adaptive bandwidth estimation, contrast stretching, and morphological filtering** to segment food images effectively. The final evaluation is performed using the **Mean Intersection over Union (mIoU) metric**.

## Objectives
- **Develop an adaptive Mean Shift-based segmentation model** for food images.
- **Leverage color space transformations** to enhance segmentation features.
- **Improve segmentation accuracy** using morphological post-processing.
- **Evaluate segmentation quality** using the **mIoU metric**.

## Key Goals
- Convert images from **BGR to HSV** color space for improved feature extraction.
- Apply **contrast stretching on Hue channel** for better segmentation accuracy.
- Implement **Mean Shift clustering** to group similar pixels.
- Use **Median Filtering** to refine the segmentation results.
- Compute **mIoU score** to evaluate segmentation accuracy.

## Tools & Technologies
- **Python**: Core programming language.
- **OpenCV**: Image processing functions.
- **Scikit-Image**: Feature extraction & transformations.
- **Scikit-Learn**: Clustering algorithms.
- **Matplotlib**: Data visualization.
- **NumPy & Pandas**: Data manipulation.

## Workflow Highlights
1. **Image Preprocessing**:
   - Convert images from **BGR to HSV**.
   - Perform **histogram analysis** to examine color distribution.
2. **Feature Extraction & Enhancement**:
   - Apply **contrast stretching on the Hue channel**.
3. **Mean Shift Clustering for Segmentation**:
   - Estimate bandwidth dynamically using `estimate_bandwidth`.
   - Perform clustering with `MeanShift` algorithm.
4. **Post-Processing**:
   - Apply **Median Filtering** to remove noise and refine segmentation.
   - Convert segmentation results into **Binary Masks**.
5. **Evaluation**:
   - Compute **mIoU score** for segmentation accuracy.

## Insights
- **Mean Shift clustering effectively segments food items** in images.
- **Contrast stretching improves segmentation accuracy** by highlighting color variations.
- **Adaptive bandwidth estimation** helps handle complex food textures.
- **mIoU score of 0.9501 confirms high segmentation precision**.

## Dataset Details
- **Source**: Food image dataset with various food categories.
- **Formats**: JPG, PNG images.
- **Processing**: Resized, normalized, and color-transformed.

## Getting Started
### Prerequisites
- Python 3.x
- OpenCV, Scikit-Image, Matplotlib, Scikit-Learn, NumPy, Pandas

## Results

- **Achieved high segmentation accuracy** with an **mIoU score of 0.9501**.
- **Mean Shift clustering effectively separates food regions** from backgrounds.
- **Post-processing using Median Filtering enhances segmentation quality**.
