# acppred

By Hadassa Ortiz

a tool to predict anticancer peptides

## Setup

```
$ make setup
```
## Project structure
* environment.yml -> list of dependencies and requirements
* requirements.txt -> all the dependencies needed to project work properly
* Makefile -> short command for making up environment
* models.py -> file with the code to a predictive model for anticancer peptides, it utilizes a database with positive and negative peptides obtained from antiCP platform. This file contains the core of ACPPred tool.
* predict.py -> file containing the predictive tool for anticancer peptides. This code loads the trained model and use its parameters to predict the anticancer potential for an inputed sequence. Returning the result with a probability of the anticancer activitiy of the peptide.
* train.py -> Trains the model for predicting anticancer peptides. It uses the Random Forest Classifier from scikit learn to estimate the positive and negative peptides.
