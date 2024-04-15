[![license](https://img.shields.io/badge/License-BSD%202--Clause-blue.svg)](https://github.com/bionicvisionlab/2024-Temporal-Model/blob/master/LICENSE)


# Predicting the temporal dynamics of prosthetic vision

Please cite as:

> Y Hou, L Pullela, J Su, S Aluru, S Sista, X Lu, M Beyeler (2024). Predicting the temporal dynamics of prosthetic vision. *46th Annual International Conference of the IEEE Engineering in Medicine & Biology Society (IEEE EMBC)*

Code for "Predicting the temporal dynamics of prosthetic vision" at IEEE EMBC 2024.

## Setup
To run the notebook, please install the required Python packages via pip:

```
pip install -r requirements.txt
```

## File description
- ```baseline_training.ipynb``` and ```baseline_evaluation.ipynb```: baseline model training and evalution. Code adapted from Avraham, David, et al. “Retinal Prosthetic Vision Simulation: Temporal Aspects.” Journal of Neural Engineering, vol. 18, no. 4, IOP Publishing, Aug. 2021, p. 0460d9, doi:10.1088/1741-2552/ac1b6c.
- ```exponential_cross_subject.ipynb```: Exponential model trained and evaluted using leave-one-subject-out cross-validation. 
- ```exponential_cross_condition.ipynb```: Exponential model trained and evaluted using leave-one-condition-out cross-validation. 
- ```FFT_cross_subject.ipynb```: FFT model trained and evaluted using leave-one-subject-out cross-validation. 
- ```FFT_cross_condition.ipynb```: FFT model trained and evaluted using leave-one-condition-out cross-validation. 
