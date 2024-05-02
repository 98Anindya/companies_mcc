# Companies Multi-class Classification

Multi-class classification modeling using companies financial dataset.

## Business background
* Based on company financials, classify each company into a performance cluster.

## Scope
* Based on a company financials labeled dataset, I was tasked with creating a machine learning multi-class classifier prediction model.

## Plan
### Metrics

## Data Acquisition & Understanding
* The original or raw dataset that was provided is `tab_data.csv`.
* #TODO: Describe your raw dataset as an e.g. in this [project report](https://github.com/Azure-Samples/MachineLearningSamples-TDSPUCIAdultIncome/blob/master/docs/deliverable_docs/ProjectReport.md)

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
#### Final or Current state
* Code File - 4a_New_Test_Modified_Cleaned_1.ipynb[Purpose - To deploy and test Multi Class Classification Models on the Bottstrapped version of Cleaned Data (To address the problem of class imbalnce each sample has 1200 data points )]
* Data File Used - 'Modified_Cleaned_1.csv'

* Code File - 4b_Multi_Class_Classification_Minimum.ipynb [Purpose - To deploy and test Multi Class Classification Models to address the class imbalance problem without bootstrapping by selecting the minimum number of datapoints possible for all unique classes in case or the original and cleaned datasets  ]
* Data Files Used - Modified_minimal.csv & 'Modified_Cleaned_minimal.csv'
  
### Feature Engineering
### Model Training
### Model Evaluation


