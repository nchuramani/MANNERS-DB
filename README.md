# Continually learning social appropriateness of robot actions under uncertainty
This repo contains all source code for the dissertation conducted in the Advanced computer science programm at Cambridge

## The code of this prooject can be seprated in three parts:
### Scripts for data structuring and data analysis of the created and labelled SARDA dataset:
#### The scripts in this part are found i the data folder and includes:
- data_analysis.ipynb\
Containing all statistical data analysis
- data_structuring.ipynb\
Cleaning and structuring the data from the Prolific platform befre saving it as csv.
### An extension of the Uncertainty-guided continual learning work by Ebrahimi et al. [1]:
#### The scripts in this part includes:
- UCB_modified.py\
The original work of Ebrahimi et al. with modifications to the loss function and some minor modifications to record the training process. The "loss" method is our 
work which fascilitates for regression, makes sure the correct output from the model is used to compute the loss and allow for aleatoric uncertainty to be obtained.
- Dataloaders\
The structure of the dataloaders used by Ebrahimi et al. is kept, but modifications are made to fit the SARDA dataset presented in our work.
- training.py\
The structure of the training script used by Ebrahimi et al. is kept, but modifications are made to fit the parameters and dataloaders necessary for our work.
### An evaluation of the predictive performance:
#### The scripts in this part includes:
- Evaluation.ipynb\
This is the main evaluation notebook where the epistemic uncertainty is obtained and performance is evaluated.
- temp_eval.ipynb\
A notebook used to investigate the model performance at different stages of the Continua learning.



[1] Ebrahimi, Sayna, et al. "Uncertainty-guided continual learning with bayesian neural networks." arXiv preprint arXiv:1906.02425 (2019).
