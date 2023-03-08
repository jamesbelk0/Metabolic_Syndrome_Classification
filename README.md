# Metabolic_Syndrome_Classification
## Discovering the health trends that lead to the metabolic syndrome

**James Belk**: Due to my experience in the health and fitness field this issue is incredibly important to the longevity to an individuals life-span and standard of living. Have a better understanding of the markers that can lead to an individuals development of a metabolic disease can help prevent them from occuring. Heart disease, diabetes, and hypertension are preventable to an extent and knowledge is power.

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
  <img src = "https://github.com/jamesbelk0/Metabolic_Syndrome_Classification/blob/33c71fc247592bd08e854b2ba0c78d4871090508/bmi.png">
  <img src = "https://github.com/jamesbelk0/Metabolic_Syndrome_Classification/blob/9849dad7828c5dd6d2a4b79daed4239a0d9b3ab3/waistcirc.png">
</p>

The chart above shows the breakdown of the individuals with a metabolic syndrome. 

- As clearly shown, the BMI and Waist Circumference of the individuals with a metabolic syndrome disease have significantly higher than those without the markers. While BMI is an archaic approach to health markers, it still shows a snapshot of an individuals health. This combined with an individuals blood glucose levels and waist circumference can help present a fuller picture of an individuals health. 
  - The CDC lists that a 'healthy' BMI can range anywhere from 18.5 to 24.9. This means the individuals in the 25-30+ range show a greater risk for health risks.

### Machine Learning Using the Following Models:
  - Logistic Regression Model
  - KN Neighbors Classifier Model
  - Random Forest Classifier Model
  - XGBoost Model
## Models Evaluated & Results
- Logistic Regression Model (Testing Set):
  - Precision: .83
  - Recall: .91 
  - F1-Score: 87 
  - Accuracy: .82

- KnNeighbor Classifier Model (Testing Set):
  - Precision: .82
  - Recall: .92 
  - F1-Score: 87 
  - Accuracy: .81

- Random Forest Classifier Model (Testing Set):
  - Precision: .88
  - Recall: .92
  - F1-Score: .90 
  - Accuracy: .87
 - XGBoost Classifier Model (Testing Set):
   - Precision: .91
   - Recall: .94
   - F1-Score: .93 
   - Accuracy: .90
 
 - The final model chosen was a `XGBoost` tuned with the max_depth tuned to 8, n_estimators to 140 and max_leaves to 9.
   - The False Positive rate is .055.
   - The Falst Negative rate is .19.
   - The Accuracy for this modelis at 90%.
 
# Business Solution
 - The XGBoost model would allow for a more confident diagnosis for the individual and possibly prevent the hospital or practice from missing a diagnosis based on previous markers. If an individuals blood glucose levels, waist circumference, or BMI are tracking along with the markers in the dataset the chances of the individual being at risk are higher. 
 - My recommendation would be to collect this data and compare findings further expanding our knowledge and preventing possible misdiagnosis in the future. 
For any additional questions, please contact **jamesbelk0@gmail.com**
