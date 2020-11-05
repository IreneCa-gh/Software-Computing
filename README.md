# Software-Computing exam
Code for the exam of the programming course of the physics department of the university of Bologna.

Here are proposed two different approaches for the classification of events taken from a dataset provided by the ATLAS experiment at CERN for 
the Kaggle Higgs Challenge.

## Dataset
The dataset was simulated by the official ATLAS full detector simulator. It reproduced the random proton-proton collisions and the measures 
of the resulting particles by a virtual model of the detector.

The signal sample corresponds to the events in which the Higgs boson decays into two taus (H → τ τ ). 

The background sample was generated by 
the three dominant background processes:
- Z → τ τ production
- t t̄  events with a hadronic τ and a leptonic τ
- W boson decays.

## Classification algorithms
The goal of this project is to get an introduction to ML algorithms with the classification of the events into signal or background.
Two different approaches were developed to classify the events.
- A model based on three Deep Neural Networks.
- A boosted decision tree provided by the Xgboost library.


The performance of the two algorithms is evaluated by computing the Approximate Median Significance (AMS) score, which is defined as
 	
![alt tag](https://github.com/IreneCa-gh/Software-Computing/blob/master/Images/AMSfunc.png)
 	
## External links
Higgs Kaggle Challenge on [Kaggle platform](https://www.kaggle.com/c/higgs-boson).

Open data: http://opendata.cern.ch/record/328


## Software and libraries required
- Python 3
- numpy
- pandas
- Scikit-learn: Python’s open source machine learning library
- matplotlib
- Keras
- XGBoost
- requests


## Note
The idea of developing a method that could be applied for the Higgs Boson Machine Learning Challenge was derived from the collaboration
between the universities of Dortmund and of Bologna. In that preceding project we only worked on the algorithm based on the Neural Networks.
Afterwards the original code have been reorganized (to improve the readability) and the classification has been a bit improved. 
Moreover the BDT analysis have been added and the documentation have been written.