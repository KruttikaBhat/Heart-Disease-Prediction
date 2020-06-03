
# Heart-Disease-Prediction
Dataset used: Heart Disease UCI. 
Source : https://www.kaggle.com/ronitf/heart-disease-uci  

## Dataset description:
This is a subset of the original dataset containing 13 attributes.
1. age
2. sex
3. chest pain type (4 values)
4. resting blood pressure
5. serum cholestoral in mg/dl
6. fasting blood sugar > 120 mg/dl
7. resting electrocardiographic results (values 0,1,2)
8. maximum heart rate achieved
9. exercise induced angina
10. oldpeak = ST depression induced by exercise relative to rest
11. the slope of the peak exercise ST segment
12. number of major vessels (0-3) colored by flourosopy
13. thal: 3 = normal; 6 = fixed defect; 7 = reversable defect

The goal of the analysis is to predict the presence of a heart disease in a patient. 
(0 = false && 1 = true)

## Analysis
We have performed Preprocessing, Descriptive Analytics and Predictive Analytics on the dataset. 
(Refer to the jupyter notebooks respectively)

The original dataset is titled "**heart.csv**". After preprocessing, the dataset is stored in "**after_preprocessing.csv**" that is used for further analysis.

Eight different **models** were trained and tested on the dataset for the prediction of heart disease. These models are stored separately in "**models**" folder. The training and testing accuracy of the models can be found in "**model_results.csv**".

### Preprocessing
The shape of the data consists of 303 rows and 14 columns with no null/missing values and one duplicate record.
|Attribute | Datatype |
|---------|--|
|age | int64 |
| gender | int64 |
| chest_pain_type | int64 |
| resting_bp | int64 |
| cholesterol | int64 |
| fasting_blood_sugar | int64 |
| resting_ecg | int64 |
| max_heart_rate | int64 |
| angina | int64 |
| st_depression | float64 |
| fluorosopy_vessels | int64 |
| thalassemia | int64 |
| target | int64 |

All the columns are either integers or float values. This is required for many machine learning algorithms. As there are no categorical columns, encoding is not done.

The modified dataset is saved to "**after_preprocessing.csv**" for further analysis.

### Descriptive Analytics
####  Univariate Analysis
In this analysis we look at individual attributes. For example,

**Target :**

Percentage of Patients with no Heart Disease: 45.70%

Percentage of Patients with Heart Disease: 54.30%

**Gender :**

Percentage of female patients : 31.79%

Percentage of male patients: 68.21%

#### Bivariate Analysis
In this analysis we consider the relationship between 2 attributes.
#### Multivariate Analysis
Analysis on multiple variables by analysing their correlation and the corresponding heat map.

*The analysis of all the attributes can be looked at in "**Descriptive Analysis.ipynb**"*

### Predictive Analytics

 - Logistic Regression
 - KNN Classification
 - Support Vector Machine
 - Naive Bayes
 - Decision Tree
 - Random Forest
 - Perceptron
 - Stochastic Gradient Descent
 
These models have been implemented ("**Predictive Analysis.ipynb**") for predictive analysis.
