# Breast-cancer-prediction
predicting breast cancer using k nearest neighbors algorithm
# Breast Cancer Classification using K-Nearest Neighbors (KNN)

## Project Overview
This project focuses on classifying breast cancer tumors as **Malignant** or **Benign** using the **K-Nearest Neighbors (KNN)** machine learning algorithm.

The goal is to build a classification model that can accurately predict cancer diagnosis based on features extracted from breast mass images.  
This project demonstrates a complete **machine learning workflow**, including data preprocessing, model training, hyperparameter tuning, and evaluation.

---

## Dataset Overview

### Dataset Name
**Breast Cancer Wisconsin (Diagnostic) Dataset**

### Description
The dataset contains features computed from digitized images of fine needle aspirates (FNA) of breast masses.  
These features describe characteristics of the cell nuclei present in the image, such as texture, radius, smoothness, and symmetry.

The dataset is commonly used for **binary classification problems** in healthcare and machine learning.

### Target Variable
- **Diagnosis**
  - `M` → Malignant (Cancerous)
  - `B` → Benign (Non-cancerous)

---

### Feature Description
Each feature is computed for cell nuclei and represented in three forms:

- **Mean** – Average value of the feature  
- **Standard Error (SE)** – Variation of the feature  
- **Worst** – Largest (worst) value of the feature  

---

### Main Feature Groups

#### 1. Radius
- Mean, SE, and worst radius of cell nuclei

#### 2. Texture
- Mean, SE, and worst texture (gray-scale variation)

#### 3. Perimeter
- Mean, SE, and worst perimeter

#### 4. Area
- Mean, SE, and worst area

#### 5. Smoothness
- Mean, SE, and worst smoothness

#### 6. Compactness
- Mean, SE, and worst compactness

#### 7. Concavity
- Mean, SE, and worst concavity

#### 8. Concave Points
- Mean, SE, and worst concave points

#### 9. Symmetry
- Mean, SE, and worst symmetry

#### 10. Fractal Dimension
- Mean, SE, and worst fractal dimension

---

### Columns Dropped
- `id` – Unique identifier (not useful for prediction)

---

## Data Preprocessing
- Dropped non-informative columns
- Encoded target variable (`M` → 1, `B` → 0)
- Scaled features using **StandardScaler**
- Split data into training and testing sets

---

## Model Used

### Machine Learning Algorithm
- **K-Nearest Neighbors (KNN)**

### Key Parameters
- `n_neighbors (k)` optimized using accuracy comparison
- Distance-based classification

---

## Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

---

## Train-Test Split
- Training data: 80%
- Testing data: 20%

---

## Results
The KNN model achieved high classification accuracy, demonstrating its effectiveness for breast cancer diagnosis prediction when combined with proper feature scaling.

---

## Conclusion
This project highlights the application of the KNN algorithm for medical diagnosis classification tasks.  
With appropriate preprocessing and tuning, KNN performs well in distinguishing between malignant and benign tumors.

---

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib / Seaborn
- Scikit-learn
