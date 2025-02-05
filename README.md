# AI-Model-for-detection-of-Inflammation-in-bowel
This projects is focused on using pretrained models to detect and predict the scores of inflammation in bowel (rectum and sigmoid) region
Endoscopic Score Prediction Model

Project Overview

This project aims to predict endoscopic scores of inflammation in the bowel and rectum using endoscopic images and videos. We utilized a comprehensive dataset of over 600 patients, including endoscopic scores linked to corresponding images.

Data Description

Patient Data: 600+ patient records

Data Types:

Endoscopic videos and images in .mat files

Electronic Health Records (EHR) with endoscopic scores in Excel files

Frameworks and Libraries

Frameworks: TensorFlow, PyTorch

Libraries: NumPy, Pandas, Matplotlib, Seaborn

Methodology

1. Data Analysis & Exploration

Conducted initial data analysis to understand variable distributions.

Performed Exploratory Data Analysis (EDA) for deeper insights.

2. Dataset Preparation

Created a custom dataset class to:

Read filenames from the Excel sheet.

Match and load corresponding .mat files.

Extract 15 frames per video.

Retrieve endoscopic scores from the EHR dataset.

3. Data Augmentation

Applied transformations:

Resize

Re-crop

Normalize

Convert to tensor format

4. Data Splitting

Divided data into training and testing sets

Batch Size: 15

Models Used

Generic Pre-trained Models

DenseNet (tuned)

EfficientNet (tuned)

Endoscopic Specialized Pre-trained Models

SeResNet50

DINOv2

Vision MAE

Training Details

Epochs: 20

Hardware: GPU utilized

Evaluation Metrics

Training & Validation Loss

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R-squared (R²)

Mean Absolute Error (MAE)

Variance

Mean Error (ME)

Visualization

Residual Plots

Distribution Plots

Actual vs Predicted Scores

Heatmaps

Training & Validation Loss over Epochs

Training & Validation RMSE over Epochs

Model Comparison

Compared performance of generic models with specialized endoscopic models.

Highlighted key differences in accuracy, efficiency, and robustness.

Results

Detailed performance analysis based on the above metrics and visualizations.

Insights into which model architecture performs best for endoscopic score prediction.

Future Work

Further tuning of specialized models

Integration with other real-time endoscopic data for predictive analysis

Contact

For any questions or collaborations, please reach out to me
