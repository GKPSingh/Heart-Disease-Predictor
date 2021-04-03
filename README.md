# Heart Disease Predictor
<img src="https://user-images.githubusercontent.com/65918602/113466784-603c1200-940c-11eb-8fd3-45dc8836f7c0.jpg" width="900" height="400">

## Introduction
This project is dedicated to the prediction of heart disease among the individuals based on the different characteristics 
of their health condition by using <b>Data Science and Machine Learning</b>.

Following Approach will be implemented:
* Problem definition
* Data
* Evaluation
* Features
* Modelling
* Experimentation

## Problem Definition
Machine Learning can play an important role in predicting healthcare, e.g. predicting hearth disease, chances of getting blood cancer etc. Such information, if predicted well in advance; can provide important insights to physicians, who can then adapt their diagnosis and treatment per patient basis.
So I want to test if based on the health parameters, will it be possible to predict whether the individual has the heart disease or not? Also with what accuracy such predictions can be made?

## Data Collection
The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease
This database contains 76 attributes, but all published experiments refer to using a subset of 14 of them. In particular, the Cleveland database is the only one that has been used by ML researchers to
this date. The "goal" field refers to the presence of heart disease in the patient. It is integer valued from 0 (no presence) to 4.
<br /><br />
<img src="https://github.com/GKPSingh/Heart_Disease_Predictor_Model/blob/main/images/data-shot.png" width="900" height="400">

## Data Attributes' / Features' Information
+ age - age in years
+ sex (2 values)
    - 0 = female
    - 1 = male
+ cp - chest pain type (4 values)
    - 0: Typical angina: chest pain related decrease blood supply to the heart
    - 1: Atypical angina: chest pain not related to heart
    - 2: Non-anginal pain: typically esophageal spasms (non heart related)
    - 3: Asymptomatic: chest pain not showing signs of disease
+ trestbps - resting blood pressure (in mm Hg on admission to the hospital). anything above 130-140 is typically cause for concern
+ chol - serum cholestoral in mg/dl. serum = LDL + HDL + .2 * triglyceride above 200 is cause for concern
+ fbs - fasting blood sugar > 120 mg/dl. '>126' mg/dL signals diabetes (2 values)
    - 1 = true
    - 0 = false
+ restecg - resting electrocardiographic results (3 values)
    - 0 = Nothing to note
    - 1 = ST-T Wave abnormality
        - can range from mild symptoms to severe problems
        - signals non-normal heart beat
    - 2: Possible or definite left ventricular hypertrophy
        - Enlarged heart's main pumping chamber
+ thalach - maximum heart rate achieved
+ exang - exercise induced angina (2 values)
    - 0 = no
    - 1 = yes
+ oldpeak - ST depression induced by exercise relative to rest
+ slope - the slope of the peak exercise ST segment (3 values)
    - 0 =  Up sloping: better heart rate with exercise (uncommon)
    - 1 = Flat sloping: minimal change (typical healthy heart)
    - 2 = Down sloping: signs of unhealthy heart
+ ca - number of major vessels (0-3) colored by flourosopy
+ thal - thalium stress result (7 values)
    - 1 - 3 = normal
    - 6 = fixed defect: used to be but ok now
    - 7 = reversible defect: no proper blood movement when exercising
+ target (2 values)
    - 0 = no
    - 1 = yes

## Important Libraries
I imported several libraries for the project:
+ numpy: To work with arrays
+ pandas: To work with csv files and dataframes
+ matplotlib: To create charts
+ seaborn: To create different category charts
+ train_test_split: To split the dataset into training and testing data
<br /><br />
<img src="https://github.com/GKPSingh/Heart_Disease_Predictor_Model/blob/main/images/heat-map.png" width="900" height="400">

## Approach
1. Data Wrangling
2. Exploratory Data Analysis (EDA) on the data set.
3. For modeling, I have identified 3 models to try: 
    - Logistic Regression
        - Predict the label of a data point by linear function
    - K-Nearest Neighbors
        - Predict the label of a data point by
            - Looking at the 'k' closest labeled data points
            - Taking a majority vote
    - Random Forest
        - Predict the label of a data point by ensembling decision trees, which is correct for decision trees' habit of overfitting.
4. Test size of Train-Test-Split is set to 20%

