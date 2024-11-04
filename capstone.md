# Biomedical Data Science Capstone Project: Predicting Heart Disease Across Diverse Populations

This project aimed to evaluate the robustness and generalizability of a heart disease prediction model using the UCI heart disease dataset. The dataset includes clinical data from four regions, with 14 features like age, sex, chest pain type, cholesterol, and maximum heart rate. By training and testing the model across different regions, this project sought to minimize bias and improve detection accuracy across diverse populations.

## Project Overview

### 1. Data Exploration and Preprocessing
- **Exploratory Analysis**: Conducted analysis to understand feature distributions and identify data biases. Found missing cholesterol values predominantly in the Switzerland dataset.
- **Data Cleaning**: Imputed missing values, removed unreliable features, and encoded categorical variables to ensure compatibility with machine learning models.

### 2. Model Development
- **Model Used**: Logistic regression model trained on Cleveland data with an 80/20 train-test split and tested on the other regions.
- **Initial Results**: Achieved an 80.3% accuracy on the Cleveland testing set, with similar performance in other regions, indicating initial model robustness.

### 3. Performance Evaluation
- **Evaluation Metrics**: Generated confusion matrices and classification reports for each region. Found recall discrepancies for predicting heart disease, especially in the Virginia dataset.
- **Best Performance**: Highest accuracy was achieved on the Hungarian dataset (81.57%), though recall for positive cases in Virginia was lower (31.37%).

### 4. Feature Importance
- **Significant Predictors**: Identified sex, chest pain type, and maximum heart rate as key predictors of heart disease, with cholesterol showing a negative coefficient.

## Conclusion and Future Directions
This project demonstrated that data quality and feature standardization are essential for model generalizability across regions. Future work could involve testing additional models and incorporating region-specific medical practices and family history data to improve heart disease prediction accuracy.
