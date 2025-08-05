
# Computer Vision Assignment 

## 📌 Overview
This repository contains solutions for **Assignment 2 of Computer Vision (CSL536)**. The tasks involve implementing various image processing and computer vision techniques, including morphological operations, clustering, feature detection, Hough transforms, and background subtraction.

---

## ✅ Problem Statements
1. **Top-hat/Bottom-hat Filtering & Thresholding**
   - Preprocess `morf_test.png` using top-hat or bottom-hat filtering.
   - Estimate and subtract background.
   - Apply global thresholding.
   - Optionally apply noise filtering and morphological operations to improve segmentation.

2. **Image Segmentation using K-Means & Mean Shift**
   - Segment `white-flower.png`, `butterfly.jpg`, and `camel.jpg` using:
     - K-Means clustering
     - Mean Shift clustering
   - Compare results of both methods.

3. **Corner Detection**
   - Detect corners in a chessboard image using **Harris Corner Detector**.

4. **Hough Transform for Lines & Circles**
   - Detect **lines** in a chessboard image.
   - Detect **circles** in `coins.jpg`.

5. **Feature Matching using SIFT**
   - Match an object between two images (`image1.png` and `image2.png`).
   - Use SIFT for feature detection and **Brute-Force Matching**.

6. **Moving Vehicle Detection**
   - Identify moving vehicles using **Median Differencing Background Subtraction**.
   - Test on `traffic.mp4`.
   - Analyze performance based on results.

---

## 🛠 Technologies Used
- **Python 3**
- **OpenCV (opencv-python & opencv-contrib-python)**
- **NumPy**
- **Matplotlib**
- **Scikit-learn** (for KMeans)

---

## 📂 Repository Structure
```
├── CV_Assignment_2.ipynb   # Jupyter Notebook with all solutions
├── CV_Assignment_2_WS_2024.pdf  # Problem Statement
├── images/                 # Folder for input images 
├── outputs/                # Folder for output results 
└── README.md
```

---

## ▶ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/CV-Assignment-2.git
   cd CV-Assignment-2
   ```
2. Install dependencies:
   ```bash
   pip install opencv-python opencv-contrib-python numpy matplotlib scikit-learn
   ```
3. Open Jupyter Notebook:
   ```bash
   jupyter notebook CV_Assignment_2.ipynb
   ```
4. Run each cell to reproduce results.

---

## 📥 Input Images & Videos
Place all input files in the `images/` folder:
- `morf_test.png`
- `white-flower.png`, `butterfly.jpg`, `camel.jpg`
- `chessboard.jpg`, `coins.jpg`
- `image1.png`, `image2.png`
- `traffic.mp4`

---

## 📤 Output Results
Place output results in the `outputs/` folder.  
Add examples in the README below for reference:

### Q1 – Morphological Processing
_Input:_  
![morf_test.png](images/morf_test.png)

_Output:_  
![Q1_result.png](outputs/Q1_result.png)

---

### Q2 – KMeans vs Mean Shift Segmentation
_Input:_  
<p align="center">
  <img src="images/white-flower.png" alt="White Flower" width="250"/>
  <img src="images/butterfly.jpg" alt="Butterfly" width="250"/>
  <img src="images/camel.jpg" alt="Camel" width="250"/>
</p>


_Output:_  
KMeans:  
![Segmentation](outputs/output_segmentation.png)  


---

### Q3 – Harris Corner Detection
![Q3_result.png](outputs/Q3_result.png)

---

### Q4 – Hough Transform
Lines:  
![Q4_lines.png](outputs/Q4_lines.png)  
Circles:  
![Q4_circles.png](outputs/Q4_circles.png)

---

### Q5 – SIFT Feature Matching
![Q5_result.png](outputs/Q5_result.png)

---

### Q6 – Moving Vehicle Detection
_Add a GIF or short video:_  
![Q6_output.gif](outputs/Q6_output.gif)

---

## 📈 Results & Observations
- **Q1:** Background estimation and morphological filtering significantly improved thresholding results.
- **Q2:** Mean Shift produced more accurate segmentation for complex regions compared to KMeans.
- **Q3:** Harris Corner Detector successfully detected chessboard corners.
- **Q4:** Hough Transform effectively detected both lines and circles.
- **Q5:** SIFT feature matching accurately matched keypoints across two images.
- **Q6:** Median differencing was effective for moving vehicle detection but may fail under shadows and lighting changes.

---

## ✅ Next Steps
- Add images and videos in respective placeholders.
- Push repository to GitHub.
