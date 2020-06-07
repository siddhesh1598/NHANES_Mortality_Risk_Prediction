# NHANES Mortality Risk Prediction

A Risk Prediction model to detect the mortality of the patients. 

## Getting Started

Clone the project repository to your local machine, then follow up with the steps as required.

## Requirements

After cloning the repository, install the necessary requirements for the project.
```
pip install -r requirements.txt
```

## Implementation

The dataset used is the [NHANES Epidomology Dataset](https://wwwn.cdc.gov/nchs/nhanes/nhefs/default.aspx/). **Mean Imputation** is used to fill in the missing values. The dataset is then trained on **Random Forest Classifier** and the best parameters are computed by using **Holdout Grid Search** method. The **shap** library is used to determine the importance of the attributes in the dataset and their weightage in determining the risk of the patients. Also, the dependency between the attributes is plotted by using **shap**.

The **util.py** code is taken from [AI for Medical Prognosis](https://www.coursera.org/learn/ai-for-medical-prognosis) Course by Deeplearning.ai. It contains the code to load the NHANES dataset and to calculate the C-Index of the data.


## Authors

* **Siddhesh Shinde** - *Initial work* - [SiddheshShinde](https://github.com/siddhesh1598)


## Acknowledgments

* Dataset: [NHANES Epidomology Dataset](https://wwwn.cdc.gov/nchs/nhanes/nhefs/default.aspx/) <br>
Dataset by **Deeplearning.ai**. (AI for Medical Prognosis Course by Deeplearning.ai on Coursera [AI for Medical Prognosis](https://www.coursera.org/learn/ai-for-medical-prognosis))
