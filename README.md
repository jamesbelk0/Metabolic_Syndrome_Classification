# Metabolic_Syndrome_Classification
## Discovering the health trends that lead to a metabolic syndrome

**James Belk**: 

<p align = "center"> 
  <img src = "https://github.com/jamesbelk0/Metabolic_Syndrome_Classification/blob/d940718f557a48ff4e9829a3ee96666cd524176b/metabolic-syndrome.jpg">
</p>

### Business problem:

Discover the risk of an individual to have a metabolic syndrome. 

### Data:
Metabolic Syndrome Dataset - https://data.world/informatics-edu/metabolic-syndrome-prediction
For this dataset, there are 2,401 rows and 15 columns

### Data Dictionary:

* seqn - Acts as ID 
* age - numeric value for the age of the individual
* sex - gender
* martial - what is the marital status
* income - how much an individual makes a month
* race - ethnicity
* waistcirc - size of the individuals waist
* bmi - dated way to measure body fat percentage
* albuminuria - sign of kidnet disease
* uralbcr - need to do more research
* uricacid - percentage of broken down substances
* bloodglucose - blood test to screen for sugar
* hdl - "good" cholesterol
* triglycerides - type of fat lipid
* metabolicsyndrome - cluster of conditions that occur together, increaseing risk of heart disease, stoke, and type 2 diabetes

## To prepare this data, the data was cleaned of extra rows and unneeded columns.The following processes were performed:

### Exploratory Data Analysis

 - During the exploratory data analysis, a bar chart and histogram were used to visualize the markers of a metabolic syndrome.
 - This provides a better understanding of the quantity of each for comparisons later.
 
 <p align = "center"> 
  <img src = "https://github.com/jamesbelk0/Metabolic_Syndrome_Classification/blob/1a7e1961bd2ba3a1c8d21a338d22c46dcc8b4649/bloodglucose_levels.png">
</p>

The chart above shows the breakdown of blood glucose levels, a major marker for a metabolic syndrome. 

- The median of the dataset is at a bloodglucose level of 99 which is the normal rate of a fasting blood glusocse level.
## Explanatory Visuals

<p align = "center"> 
  <img src = "https://github.com/jamesbelk0/Metabolic_Syndrome_Classification/blob/1a7e1961bd2ba3a1c8d21a338d22c46dcc8b4649/meta_syndrome_bar.png">
</p>

The chart above shows the breakdown of the individuals with a metabolic syndrome. 

- As clearly shown, the BMI of the individuals with a metabolic syndrome disease have significantly higher BMI than those without. While BMI is an archaic approach to health markers, it still shows a snapshot of an individuals health. This combined with an individuals blood glucose levels and waist circumference can help present a fuller picture. 
  - The CDC lists that a 'healthy' BMI can range anywhere from 18.5 to 24.9. This means the individuals in the 25-30+ range show a greater risk for health risks.

### Machine Learning Using the Following Models:
  - Logistic Regression Model
  - KN Neighbors Classifier Model
  - Random Forest Classifier Model
## Models Evaluated & Results
- Linear Regression Model (Testing Set):
  - MAE: 847.1571 
  - MSE: 1,297,218.6566 
  - RMSE: 1,138.9551 
  - R2: 0.5617

- Decision Tree Regressor Model (Testing Set):
  - MAE: 1,138.5329 
  - MSE: 2,255,705.5459 
  - RMSE: 1,501.9006 
  - R2: 0.2378

- Tuned Decision Tree Regressor Model (Testing Set):
  - MAE: 762.6076 
  - MSE: 1,172,166.0943 
  - RMSE: 1,082.6662 
  - R2: 0.6039
 
 - The final model chosen was a `Tuned Decision Tree` with the max_depth tuned to 5.
 - The Mean Absolute Error was off by about `24.40`.
 - The Mean Squared Error was `54,007`.
 - The Root Meaqn Squared Error had a calculation of `25.2354`.
 

For any additional questions, please contact **jamesbelk0@gmail.com**
