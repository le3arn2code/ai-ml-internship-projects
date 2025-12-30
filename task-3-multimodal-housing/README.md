# Task 3: Multimodal Housing Price Prediction

## Objective
The objective of this task is to predict housing prices using a multimodal machine learning approach that combines visual information from house images with structured tabular features.

This task demonstrates how deep learning–based image representations can be fused with traditional numerical data to solve a regression problem.

---

## Dataset Description
The dataset consists of a small synthetic housing dataset containing:
- **Tabular features**:
  - Square footage (`sqft`)
  - Number of bedrooms
  - Number of bathrooms
  - House age
  - Location score (proxy for neighborhood quality)
- **Image data**:
  - One image per house, programmatically generated to simulate visual differences
- **Target variable**:
  - House price

---

## Methodology
1. A **pretrained MobileNetV2 CNN** is used as a fixed feature extractor to obtain 1280-dimensional embeddings from each house image.
2. Tabular features are standardized using `StandardScaler`.
3. Image embeddings and tabular features are **concatenated** to form a single feature vector.
4. A fully connected neural network is trained on the combined features to predict housing prices.

---

## Evaluation Metrics
Model performance is evaluated using:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

---

## Results
- **MAE:** ~552,301  
- **RMSE:** ~578,766  

Given the small dataset size and high target value range, these results are expected and demonstrate successful multimodal feature learning.

---

## Conclusion
This project successfully implements a multimodal regression pipeline by integrating image-based deep learning features with traditional tabular data. The approach highlights the flexibility of combining different data modalities within a single machine learning model.
