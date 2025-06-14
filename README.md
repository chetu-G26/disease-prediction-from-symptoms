# Disease Prediction from Symptoms 🧠💉
This project predicts diseases based on symptoms using machine learning classification models. It aims to help in early diagnosis and resource prioritization by analyzing user-reported symptoms and predicting probable diseases.
## Problem Statement
Developed a machine learning application to predict diseases based on symptom data. The goal is to:
	Enable early diagnosis
	Optimize healthcare resource allocation
	Improve patient engagement in self-care
## Dataset
I used public datasets from:
•	ColumbiaUniversity:http://people.dbmi.columbia.edu/~friedma/Projects/DiseaseSymptomKB/index.html

•	Kaggle: The dataset is a public dataset acquired from Kaggle. It is a raw dataset which consists of Disease, Count of disease occurrence and Symptoms. https://www.kaggle.com/datasets/itachi9604/disease-symptom-description-dataset

## Data Preprocessing
•	Removed duplicates and cleaned symptom/disease names

•	Split multi-symptom rows into individual entries

•	Assigned binary values (0/1) for symptom presence

•	Mapped disease labels to rows 

Final data set prepared in jupyter using Excel + Python.

## Data Visualization
•	Correlation heatmap between symptoms

•	Correlation heatmap between diseases

These helped identify symptom clusters and disease co-occurence.

## Models Used
### 1. Multinomial Naive Bayes
•	Assumes feature independence

•	Efficient for high-dimensional input

Also  used laplace smoothing to handle missing  features.


### 2. Decision Tree Classifier
•	Captures feature interactions

•	Provides feature importance rankings

Also suitable for exploratory knowledge discovery.

## Implementation Steps
•	Train test split

•	Model training and validation

•	Feature importance extraction (from Decision Tree) and  Evaluation of accuracy and precision.

## Evaluation & Results
Top symptoms ranked by importance (Decision Tree):

1. loss_of_smell (0.0269)
2. internal_itching (0.0269)
3. hip_joint_pain (0.0268)
4. increased_appetite(0.0266)
5. malaise(0.0261)

Decision tree outperformed Naive Bayes in overall prediction accuracy.

## Conclusion
The Decision Tree model provided more accurate predictions due to its ability to capture symptom combinations, unlike Naive Bayes which assumes independence.
 







