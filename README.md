# 📸 Smart Vision Face Attendance System

A smart attendance system powered by computer vision and facial recognition. This project detects and recognizes faces from static or real-time input to automate attendance marking, enhancing security and reducing manual effort.

## 🧠 Overview

This system performs:
- **Face Detection** using the Viola-Jones algorithm
- **Image Pre-processing** (grayscale conversion, median filtering, CLAHE)
- **Feature Extraction** with LBP, PCA, and a hybrid LBP-PCA approach
- **Classification** using distance metrics for face recognition
- **Evaluation** with accuracy metrics such as Precision, Recall, F1 Score, and more

## 🚀 Features

- 🧑‍🏫 Real-time face recognition for attendance
- 📷 Preprocessing to enhance image quality
- 💡 Hybrid feature extraction approach for improved accuracy
- 🧪 Evaluated using standard datasets (custom dataset)

## 🛠️ Technologies Used

- Python
- OpenCV
- NumPy
- scikit-learn
- Matplotlib


> Metrics computed based on comparison with human-labeled ground truth.

## 📁 Dataset

- 👨‍🎓 Custom student dataset for real-world testing

## 🧪 How It Works

### 1. Image Pre-processing
- Convert images to grayscale
- Apply median filter and CLAHE (Contrast Limited Adaptive Histogram Equalization)

### 2. Feature Extraction
- **LBP**: Captures local texture patterns
- **PCA**: Reduces dimensionality while preserving variance
- **Hybrid**: Combines LBP and PCA for better recognition

### 3. Face Detection & Recognition
- Viola-Jones for face detection
- Two-phase system: training and recognition
- Uses distance classifiers (Euclidean, Chi-Square, etc.) for matching

## 🔧 Installation

```bash
git clone https://github.com/yourusername/face-attendance-system.git
cd face-attendance-system
pip install -r requirements.txt
