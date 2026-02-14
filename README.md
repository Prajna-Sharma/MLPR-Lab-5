# MLPR-Lab-5
# Lab 5: Face Classification using Hue–Saturation Features and K-Means Clustering

##  Aim
The aim of this experiment is to implement a distance-based face classification system using colour features extracted from detected face regions. The task involves clustering faces using **K-Means clustering** and classifying a template face image based on its proximity to learned clusters.

---

## Methodology

The methodology followed in this lab consists of the following steps:

### 1. Face Detection
- Face detection is performed using **Haar Cascade Classifier** on grayscale images.
- Bounding boxes are drawn around detected faces.

### 2. Feature Extraction
- The detected face regions are converted from **BGR to HSV color space**.
- **Mean Hue and Saturation values** are extracted from each detected face.
- These values form a 2D feature vector for each face.

### 3. Clustering using K-Means
- The extracted Hue–Saturation features are clustered using **K-Means clustering**.
- The number of clusters is set to **K = 2**.
- Cluster centroids are computed and visualized.

### 4. Template Image Classification
- A template image is processed in the same way:
  - Face detection
  - HSV conversion
  - Mean Hue–Saturation extraction
- The template feature vector is classified using the trained **K-Means model**.

---

## Visualizations and Results

### 1. Face Detection Output
Detected faces are highlighted with bounding boxes.

![Face Detection Output](images/face_detection.png)

---

### 2. Hue–Saturation Feature Space
Each face is plotted in Hue–Saturation space along with cluster centroids.

![Hue-Saturation Scatter Plot](images/hs_scatter.png)

---

### 3. Clustered Faces with Template Image
The template face is plotted along with clustered faces to show its assigned class.

![Template Classification](images/template_classification.png)

---

## Key Findings
- Hue and Saturation are effective low-dimensional features for basic face grouping.
- K-Means clustering successfully separates faces into distinct clusters.
- The template image is correctly classified based on its proximity to cluster centroids.
- Visualization in HS-space helps in understanding cluster separation clearly.

---

## Conclusion
This lab demonstrates how distance-based learning techniques can be applied to image-based classification problems using simple color features. The approach highlights the importance of:
- Feature extraction
- Distance metrics
- Clustering and visualization

The experiment also reinforces the role of unsupervised learning in classification tasks when labeled data is unavailable.

---

## Tools and Libraries Used
- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn

---

## 📁 Repository Structure
