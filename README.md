# Companies Multi-class Classification

Multi-class classification modeling using companies financial dataset.

## Business background
* Based on company financials, classify each company into a performance cluster.

## Scope
* Based on a company financials labeled dataset, I was tasked with creating a machine learning multi-class classifier prediction model.

## Plan
### Metrics
* Objective was to gain a .95% accuracy for the multi class classification models or higher .

## Data Acquisition & Understanding
* The original or raw dataset that was provided is `tab_data.csv`.


### Data Exploration
* #TODO: write about the final EDA outcome
* Code File - EDA_Outlier_Removal.ipynb [Purpose- Contains Graphical representations of the variables before and after outlier removal is perfromed on the original data i.e 'tab_data.csv' ]
* Code File - EDA.ipynb [Purpose - Contains Exploratory Data analytics performed at various stages of problem solving to better understand and evaluate the data ]
* 

## Modeling

### Modeling Trials & Iterations
#### Trial-1 
* Code File - 1_Multi_Class_Classification_Original.ipynb [Purpose - To deploy and test Multi Class Classification Models on the Original Data ]
* Data File Used - `tab_data.csv`
#### Trial-2
* Code File - 2_Multi_Class_Classification_Modified.ipynb  [Purpose - To deploy and test Multi Class Classification Models on the Cleaned Data (Data cleaning performed on the original data to get new dataset ) ]
* Data File Used - 'Modified_1.csv'
#### Trial-3
* Code File - 3_New_Test_Main.ipynb [Purpose - To deploy and test Multi Class Classification Models on the Bottstrapped version of Original Data (To address the problem of class imbalnce each sample has 1200 data points )]
* Data File Used - 'Modified_tab_data.csv'
#### Final or Current state (Trial 4)
* Code File - 4a_New_Test_Modified_Cleaned_1.ipynb[Purpose - To deploy and test Multi Class Classification Models on the Bottstrapped version of Cleaned Data (To address the problem of class imbalnce each sample has 1200 data points )]
* Data File Used - 'Modified_Cleaned_1.csv'

* Code File - 4b_Multi_Class_Classification_Minimum.ipynb [Purpose - To deploy and test Multi Class Classification Models to address the class imbalance problem without bootstrapping by selecting the minimum number of datapoints possible for all unique classes in case or the original and cleaned datasets  ]
* Data Files Used - Modified_minimal.csv & 'Modified_Cleaned_minimal.csv'
  

### Model Training

* Multi Class Classification Models Used - Xgboost , Catboost , Random Forest Classifier

### Model Evaluation

* We see significant increase in the accuracy metric of the models as we progress from Trial 1 to Trial 4 . For example for Trial 1 , we observe the accuracy metrics to be Random Forest Evaluation(Accuracy: 0.6935) / XGBoost Evaluation(Accuracy: 0.7641)/CatBoost Evaluation(Accuracy: 0.7399) . For Trial 4 (Case 4a) we find the accuracy metrics to be Random Forest Evaluation(Accuracy: 0.9430555555555555) /XGBoost Evaluation(Accuracy: 0.94)/CatBoost Evaluation(Accuracy: 0.9777777777777777)


### Notes

* While evaluating the file , "Modified_Cleaned_1.csv" which was generated through bootstrapping to solve the Class imbalance problem observed , it is noticed that there is significant duplication of data . This could lead to overfitting and inaccuracies . Further investigation reveals that employment of SMOTE technique might help to resolve this issue without the inaccuracies (Yet to be deployed )
* Feature Engineering was explored , and had resulted in slight increase in accuracy but was not implemented in scale . 

