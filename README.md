**About**
---------
Machine learning model (XGBoost) for the paper:
Explainable machine learning using echocardiography to improve mortality prediction in patients with chronic coronary syndrome

In this study we have developed a machine learning model to predict five-years mortality in patients with chronic coronary syndrome (CCS) using clinical characteristics and transthoracic echocardiography (TTE) data.
This model was trained on consecutive patients with CCS who attended the outpatient clinic of Amsterdam University Medical Centers, location AMC.
The model was tested on patients who attended the outpatient clinic the Amsterdam University Medical Centers, location VUmc.

**Training**
----------
Hyperparameters used for training:            
Learning rate (eta)	[0.01, 0.03, 0.05, 0.07, 0.1]	        
Number of decision trees (n_estimators)	[100, 200, 300, 400]
Maximum depth of decision tree (max_depth)	[1,2,3,4]	   
Fraction of training data that is used to train each individual tree (subsample)	[0.7,0.8,0.9].

Optimal hyperparameters
Learning rate (eta):                                                      0.05  
Number of decision trees (n_estimators):	                                                  200  
Maximum depth of decision tree (max_depth):                                                           1  
Fraction of training data that is used to train each individual tree (subsample):               0.7  

**Requirements**
------------
Requirements
This code was run and tested on a windows-based computer with a Intel Core i5-6200 CPU (2.30 GHz, 8.00GB) with the following dependencies:

python 3.8.3
scikit-learn 1.1.3
pandas 1.5.2
numpy 1.23.5
xgboost 1.7.3.

**Required Features**
---------------
'Age' : age of patient (years)  
'BMI' : body mass index (kg/m2)  
'LV_dysfunction': left ventricular dysfunction (yes/no)  
'Lab_eGFR': estimated glomerular filtration rate (ml/min/1,73 m2)  
'TR_yesno': tricuspid regurgitation (yes/no)  
'History_of_COPD': COPD in medical history (yes/no)  
'periferal_CAD': peripheral coronary artery disease (yes/no)  
'Hartfrequentie': heart rate (beats per minute)  
'History_of_atrial_fibrillation_flutter': atrial fibrillation and\or -flutter in medical history (yes/no)  


**How to open model?**
-----------
Save file to specific folder  
filename = r'xxx\xxx\xxx\xgboost_model.pkl'  
Load model  
loaded_model = pickle.load(open(filename, 'rb'))

**Citation**
------------
We encourage researchers to use validate our machine learning model, so that we can have a cumulatively growing literature on the prediction of mortality in patients with CCS. If you use our code, please cite:

@article{Explainable machine learning using echocardiography to improve risk prediction in patients with chronic coronary syndrome,
  author = {Molenaar et al.},
  editor = {European Heart Journal - Digital Health},
  month = {xx},
  pages = {xx},
  title = {xx},
  doi = {https://doi.org/10.1093/ehjdh/ztae001},
  urldate = {xx},
  volume = {xx},
  year = {2024},
  journal = {European Heart Journal - Digital Health}
}

**contact**
------------
In case of any questions, please email to:  
m.a.molenaar1@amsterdamumc.nl or  
m.j.schuuring@amsterdamumc.nl
