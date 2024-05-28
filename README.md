# Pima Indians Diabetes Database 🩺

📄 **Paper link:** https://doi.org/10.1109/ICIRCA54612.2022.9985487

**Note:** This project was initially completed and presented during an internship at the 'Data Exposys Lab,' Bengaluru.

---

## Predicting the Onset of Diabetes

Diabetes is a chronic disease prevalent across all age groups. Early prediction can help individuals take preventive measures and manage the disease effectively. This project aims to identify whether a patient has diabetes based on diagnostic measurements.

* **Dataset Used:** The dataset, sourced from the UCI Machine Learning Repository, contains 769 records of female patients and is available on Kaggle.
* 📊 **Dataset Link:** https://www.kaggle.com/uciml/pima-indians-diabetes-database

---

## Project Methodology 📈

### Data Collection

The study uses the Pima Indians Diabetes Database from the National Institutes of Diabetes and Digestive and Kidney Diseases. The dataset includes diagnostic measurements from 768 female patients of Pima Indian heritage, with the goal of determining the presence of diabetes.

### Data Preparation

**Data Pre-Processing:**
- **Handling Missing Values:** Missing values were replaced with the median of their respective attributes using Pandas and NumPy libraries.
- **Outlier Detection and Removal:** Outliers were identified and removed using the interquartile range (IQR) method. After removing outliers, 732 values remained in the dataset.
- **Feature Engineering:** New variables were created logically and one-hot encoded. Attributes were scaled using Robust Scaler to prevent bias.

**Splitting the Data:**
- The data was split into 65% training and 35% testing datasets.

### Machine Learning Models

**K-Nearest Neighbor (KNN):**
- **Algorithm:** Used for classifying data by finding the most similar training data.
- **Optimal K Value:** Selected based on the highest accuracy from a range of K values. The optimal K value found was 16.
- **Performance:** Training accuracy was 87.21%, and testing accuracy was 82.81%.

**Random Forest Classifier (RF):**
- **Algorithm:** Uses multiple decision trees to improve prediction accuracy.
- **Performance:** Training accuracy was 92.04%, and testing accuracy was 87.89%. This model had the highest accuracy among the tested models.

**Artificial Neural Network (ANN):**
- **Architecture:** Consisted of 7 hidden layers with batch normalization and dropout to prevent overfitting. Stochastic Gradient Descent was used as the optimizer.
- **Performance:** Training accuracy was 93.08%, and testing accuracy was 86.32%.

### Evaluation Metrics

- **Precision:** Ratio of true positives to the sum of true positives and false positives.
- **Recall:** Ratio of true positives to the sum of true positives and false negatives.
- **F1-Score:** Harmonic mean of precision and recall.
- **Accuracy:** Sum of true predictions divided by the total number of predictions.

### Results

**KNN Model:**
- Precision: 87%
- Recall: 89%
- F1-Score: 88%
- Training + Testing Time: 1.43 seconds

**RF Classifier:**
- Precision: 90%
- Recall: 93%
- F1-Score: 91%
- Training + Testing Time: 1.61 seconds

**ANN Model:**
- Precision: 89%
- Recall: 91%
- F1-Score: 90%
- Training + Testing Time: 1.64 seconds

### Software Packages Used

- **Python-sci-kit-learn:** 0.24
- **Numpy:** 1.21.1
- **Pandas:** v1.3.1
- **Matplotlib:** 3.3.4
- **TensorFlow:** 2.0
- **Keras:** 2.3.0
- **Seaborn:** 0.11.1

### Advantages and Real-World Applications 🌍

- **Early Detection:** This project aids in the early detection of diabetes, allowing for timely medical intervention.
- **Preventive Measures:** Individuals can take preventive measures to manage their lifestyle and reduce the risk of developing diabetes.
- **Healthcare Support:** Doctors can use this model to identify at-risk patients and prioritize their care.
- **Business Applications:** Health insurance companies can use predictive models to assess risk and tailor their policies. Fitness and wellness programs can integrate these insights to provide personalized health plans.

## Project Advantage 🌟

The derived rules help doctors identify diabetes patients early, leading to timely intervention and treatment before the condition becomes critical. This can significantly reduce healthcare costs and improve patient outcomes.

## Citation 📝

If you use the code in this repository, please cite the following paper:
```
@INPROCEEDINGS{9985487,
author={J, Aravinda Raman and Kotian, Rakshan},
booktitle={2022 4th International Conference on Inventive Research in Computing Applications (ICIRCA)},
title={Diabetes Prognosis using Machine Learning},
year={2022},
volume={},
number={},
pages={875-882},
doi={10.1109/ICIRCA54612.2022.9985487}}
```

