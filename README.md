# Heart_Disease_Predictor_Model

### Predicting heart disease using machine learning
This notebook is dedicated to the prediction of heart disease among the individuals based on the different characteristics 
of their health condition by using Data Science and Machine Learning Models.

![Heart1](https://user-images.githubusercontent.com/65918602/113466779-5ca88b00-940c-11eb-9b0e-7580cb302b8a.jpg)

Following Approah will be implemented:

* Problem definition
* Data
* Evaluation
* Features
* Modelling
* Experimentation

#### 1. Problem Defination
Based on the health parameters, will it be possible to predict whether the individual has the heart disease or not??

#### 2. Data Collection
The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease

#### 3. Evaluation
If after modeling, the accuracy of the model to predict comes out to be more than 95%, the project will be persued further.

#### 4. Features
Information of different attributes of data is given below:

###### Create data dictionary

1. age - age in years
2. sex - (1 = male; 0 = female)
3. cp - chest pain type

   * 0: Typical angina: chest pain related decrease blood supply to the heart

   * 1: Atypical angina: chest pain not related to heart
   
   * 2: Non-anginal pain: typically esophageal spasms (non 
        heart related)
   * 3: Asymptomatic: chest pain not showing signs of   
        disease
4. trestbps - resting blood pressure (in mm Hg on admission 
             to the hospital) anything above 130-140 is  
             typically cause for    concern

5. chol - serum cholestoral in mg/dl
   * serum = LDL + HDL + .2 * triglycerides
   * above 200 is cause for concern

6. fbs - (fasting blood sugar > 120 mg/dl) (1 = true; 0 =   
   false)
   * '>126' mg/dL signals diabetes

7. restecg - resting electrocardiographic results
   * 0: Nothing to note
   * 1: ST-T Wave abnormality
       * can range from mild symptoms to severe problems
       * signals non-normal heart beat
    * 2: Possible or definite left ventricular hypertrophy
        * Enlarged heart's main pumping chamber

8. thalach - maximum heart rate achieved

9. exang - exercise induced angina (1 = yes; 0 = no)

10. oldpeak - ST depression induced by exercise relative to 
             rest looks at stress of heart during excercise unhealthy heart will stress more

11. slope - the slope of the peak exercise ST segment
    * 0: Upsloping: better heart rate with excercise  
       (uncommon)
    * 1: Flatsloping: minimal change (typical healthy heart)
    * 2: Downslopins: signs of unhealthy heart

12. ca - number of major vessels (0-3) colored by flourosopy
        * colored vessel means the doctor can see the blood 
          passing through
        * the more blood movement the better (no clots)

13. thal - thalium stress result
      * 1,3: normal
      * 6: fixed defect: used to be defect but ok now
      * 7: reversable defect: no proper blood movement when 
           excercising

14. target - have disease or not (1=yes, 0=no) (= the 
             predicted attribute)
             


#### Approach
![Hearttech](https://user-images.githubusercontent.com/65918602/113466784-603c1200-940c-11eb-8fd3-45dc8836f7c0.jpg)


1. Apply data wrangling, exploratory data analysis on the data set.
2. For modeling, apply Logistic Regression, K-Nearest Neighbors, Random Forest for this supervised learning problem.
