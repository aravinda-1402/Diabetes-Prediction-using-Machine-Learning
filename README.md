# Pima Indians Diabetes Database
Paper accepted at <b>'IEEE 4th International Conference on Inventive Research in Computing Applications (ICIRCA 2022).'</b>

<u>Note</u>: <b>The earlier version of this project was done by me as part of an internship at the 'Data Exposys Lab', Bengaluru </b>.
## Predicting the onset of diabetes

Diabetes is a type of chronic disease which is more common among the people of all age groups. Predicting this disease at an early stage can help a person to take the necessary precautions and change his/her lifestyle accordingly to either prevent the occurrence of this disease or control the disease (For people who already have the disease).
So, the objective of this project is to identify whether the patient has diabetes or not based on diagnostic measurements.

* **Dataset Used:** The dataset used has been obtained from UCI Machine Learning Repository having 769 records of Female Patients exclusively from Kaggle.

* **Dataset Link:**  [PIMA-Indian-diabetes_database](https://www.kaggle.com/uciml/pima-indians-diabetes-database)

From the domain knowledge, I have analyzed and found out the ranges of values and its effects on diabetes for each continuous variable in the dataset. Based upon these ranges we will categorize the continuous variables for implementing the learning models like KNN, Random-Forest and Artificial Neural Network and see which model provides the best accuracy in the next step. Also, we can utilize these ranges to come up with appropriate null value replacement for each independent variable.

**There are 8 independent variables:**
1.	***Pregnancies:*** No. of times pregnant.

2.	***Glucose:*** Plasma Glucose Concentration a 2 hour in an oral glucose tolerance test (mg/dl)
A 2-hour value between 140 and 200 mg/dL (7.8 and 11.1 mmol/L) is called impaired glucose tolerance. This is called "pre-diabetes." It means you are at increased risk of developing diabetes over time. A glucose level of 200 mg/dL (11.1 mmol/L) or higher is used to diagnose diabetes.

3.	***Blood Pressure:***  Diastolic Blood Pressure(mmHg) 
•	If Diastolic B.P > 90 means High B.P (High Probability of Diabetes) 
•	Diastolic B.P < 60 means low B.P (Less Probability of Diabetes)

4.	***Skin Thickness:*** Triceps Skin Fold Thickness (mm) –A value used to estimate body fat. Normal Triceps Skin-fold Thickness in women is 23mm. Higher thickness leads to obesity and chances of diabetes increases.

5.	***Insulin:*** 2-Hour Serum Insulin (mu U/ml)


6.  ***BMI:*** Body Mass Index (weight in kg/ height in m2 ) Body Mass Index of 18.5 to 25 is within the normal range BMI between 25 and 30 then it falls within the overweight range. A BMI of 30 or over falls within the obese range.

7.	***Diabetes Pedigree Function:*** It provides information about diabetes history in relatives and genetic relationship of those relatives with patients. Higher Pedigree Function means patient is more likely to have diabetes.

8.	***Age (Years)***

9.	***Outcome:*** Class Variable (0 or 1) where ‘**0**’ denotes patient is not having diabetes and ‘**1**’ denotes patient having diabetes.

**The** ***dependent variable*** **is whether the patient is having diabetes or not.**

* **Data Cleaning:** It will take place as data has got a lot of missing values. Handling missing values can be done either by replacing null values with mode, mean, median or replacing the null with a random variable.


* **Algorithms Used:**  As we have to classify the data into patients having diabetes or not, I have chosen k-nearest neighbors (KNN), Random decision forests and artificial neural networks (ANN) to see which one provides us with the best accuracy.

* **Software Package Used:** 
•	Python-scikit-learn 0.24
•	Numpy 1.21.1
•	Pandas v1.3.1 
•	Matplotlib 3.3.4 
•	TensorFlow 2.0 
•	Keras 2.3.0
•	Seaborn 0.11.1.

* **Advantage of this project:** The rules derived will be helpful for doctors to identify patients suffering from diabetes. Further predicting the disease early leads to treating the patient before it becomes critical.


