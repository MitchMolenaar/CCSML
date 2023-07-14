**About**
Machine learning model (XGBoost) for the paper:
Explainable machine learning using echocardiography to improve mortality prediction in patients with chronic coronary syndrome

In this study we have developed a machine learning model to predict five-years mortality in patients with chronic coronary syndrome (CCS) using clinical characteristics and transthoracic echocardiography (TTE) data.
This model was trained on consecutive patients with CCS who attended the outpatient clinic of Amsterdam University Medical Centers, location AMC.
The model was tested on patients who attended the outpatient clinic the Amsterdam University Medical Centers, location VUmc.

**Training**
Hyperparameters of model:                                                                                      Optimal hyperparameters:__
Learning rate (eta)	[0.01, 0.03, 0.05, 0.07, 0.1]	                                                              0.03 __
Number of decision trees (n_estimators)	[100, 200, 300, 400]	                                                   400__
Maximum depth of decision tree (max_depth)	[1,2,3,4]	                                                            1__
Fraction of training data that is used to train each individual tree (subsample)	[0.7,0.8,0.9]	                  0.7__



**Requirements**
Requirements
This code was run and tested on an Nvidia TITAN RTX GPU with the following dependencies:

python 3.8.16
torch 1.12.1+cu102
tensorboard 2.11.2
scikit-learn 1.2.1
pandas 1.5.3
numpy 1.24.1

**Citation**
We encourage researchers to use validate our machine learning model, so that we can have a cumulatively growing literature on the prediction of mortality in patients with ccs. If you use our code, please cite:

@article{xxx,
  author = {xx},
  editor = {xx},
  month = {xx},
  pages = {xx},
  title = {xx},
  doi = {xx},
  urldate = {xx},
  volume = {xx},
  year = {xx},
  journal = {xx}
} 
