# NHANES Mortality Risk Prediction

![alt text](https://github.com/siddhesh1598/NHANES_Mortality_Risk_Prediction/blob/master/thumbnail.jpg?raw=true)

A Risk Prediction model to detect the mortality of the patients. The dataset used is the [NHANES Epidomology Dataset](https://wwwn.cdc.gov/nchs/nhanes/nhefs/default.aspx/). It containes patient's attributes such as *Age,	Diastolic BP,	Poverty index,	Race,	Red blood cells,	Sedimentation rate,	Serum Albumin	Serum Cholesterol, etc.*  The code used Random Forest to predict the mortality rate. 

## Technical Concepts

**Random Forest:** Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees. <br>
More information can be found [here](https://www.researchgate.net/profile/Andy_Liaw/publication/228451484_Classification_and_Regression_by_RandomForest/links/53fb24cc0cf20a45497047ab/Classification-and-Regression-by-RandomForest.pdf)

**SHAP (SHapley Additive exPlanations):** It is a game theoretic approach to explain the output of any machine learning model. It connects optimal credit allocation with local explanations using the classic Shapley values from game theory and their related extensions. 
More information can be found [here](https://shap.readthedocs.io/en/latest/)

## Getting Started

Clone the project repository to your local machine, then follow up with the steps as required.

## Requirements

After cloning the repository, install the necessary requirements for the project.
```
pip install -r requirements.txt
```

## Implementation

**Mean Imputation** is used to fill in the missing values. The dataset is then trained on **Random Forest Classifier** and the best parameters are computed by using **Holdout Grid Search** method. The **shap** library is used to determine the importance of the attributes in the dataset and their weightage in determining the risk of the patients. Also, the dependency between the attributes is plotted by using **shap**.

The **util.py** code is taken from [AI for Medical Prognosis](https://www.coursera.org/learn/ai-for-medical-prognosis) Course by Deeplearning.ai. It contains the code to load the NHANES dataset and to calculate the C-Index of the data.

![alt text](https://github.com/siddhesh1598/NHANES_Mortality_Risk_Prediction/blob/master/SHAP_values.png?raw=true)

SHAP values (impact of attributes on model's output)


## Authors

* **Siddhesh Shinde** - *Initial work* - [SiddheshShinde](https://github.com/siddhesh1598)


## Acknowledgments

* Dataset: [NHANES Epidomology Dataset](https://wwwn.cdc.gov/nchs/nhanes/nhefs/default.aspx/) <br>
Dataset by **Deeplearning.ai**. (AI for Medical Prognosis Course by Deeplearning.ai on Coursera [AI for Medical Prognosis](https://www.coursera.org/learn/ai-for-medical-prognosis))
