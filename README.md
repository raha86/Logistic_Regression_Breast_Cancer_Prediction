# Logistic_Regression_Breast_Cancer_Prediction

# Dataset Link:
https://drive.google.com/file/d/1PqT0xwQjsyScKf50YLzoDGYDi51Pb_bs/view?usp=sharing

# Problem Statement:
Create a model to predict presence of breast cancer based on the independant variables.

# About Dataset
### Attribute Information:

1. ID number
2. Diagnosis (M = malignant, B = benign) (Target Variable)

3 - 32) Ten real-valued features are computed for each cell nucleus:
   
a) radius (mean of distances from center to points on the perimeter)  <br/>
b) texture (standard deviation of gray-scale values) <br/>
c) perimeter <br/>
d) area <br/>
e) smoothness (local variation in radius lengths)  <br/>
f) compactness (perimeter^2 / area - 1.0)  <br/>
g) concavity (severity of concave portions of the contour)  <br/>
h) concave points (number of concave portions of the contour)  <br/>
i) symmetry  <br/>
j) fractal dimension ("coastline approximation" - 1)  <br/>

The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.

All feature values are recoded with four significant digits.

# Steps Performed:
1. Performed data cleaning:
   * checked for missing values
   * checked for duplicate values
   * <b>Important finding:</b> Data is imbalanced
2. Data Manipulation:
   * Converted categorical values of 'diagnosis' column to numerical values.
3. Feature Selectiom:
   * Used <b>Correlation matrix and Heatmap</b> for feature selection.
4. Data Standarization:
   * <b>Data standardization</b> - Normalizing the features so that the samples will have the same mean and standard deviation. Used standard scaler.
   * <b>Used StandardScaler</b> for data standardization.
5. Model Building.
6. Model Evaluation:
   * Used <b>ROC-AUC Score (Receiver Operating Characteristics Area Under Curve)</b> for model evaluation.
   * As the data was imbalanced, ROC-AUC Score is one of best metrics for pereformance evaluation.
   * <b>Achieved</b> : ROC-AUC Score 0.988 (98.8%)
7. Visual Representation:

![image](https://github.com/user-attachments/assets/404c5bc3-5287-4682-8b24-dd2acca1ab43)


