[![license](https://img.shields.io/badge/License-BSD%202--Clause-blue.svg)](https://github.com/bionicvisionlab/2024-Temporal-Model/blob/master/LICENSE)


# Predicting the Temporal Dynamics of Prosthetic Vision

Code for "Predicting the Temporal Dynamics of Prosthetic Vision" at IEEE EMBC 2024.

Please cite as:

> Y Hou, L Pullela, J Su, S Aluru, S Sista, X Lu, M Beyeler (2024). Predicting the Temporal Dynamics of Prosthetic Vision. *46th Annual International Conference of the IEEE Engineering in Medicine & Biology Society (IEEE EMBC)*

Note: Y Hou and L Pullela contribute equally to this work.

In this paper, we introduced two computational models designed to accurately predict phosphene fading and persistence under varying stimulus conditions, cross-validated on behavioral data reported by nine users of the Argus II Retinal Prosthesis System.

## Setup
To run the notebooks, please install the required Python packages via pip:

```
pip install -r requirements.txt
```

## Data availability
To load the data from Perez Fornos et al., 2012, please install the stable or bleeding-edge version of [![pulse2percept](https://pulse2percept.readthedocs.io/en/latest/index.html)] via pip:
```
pip install pulse2percept
```

or

```
pip install git+https://github.com/pulse2percept/pulse2percept
```

Then load the dataset as Pandas dataframe:
```
import numpy as np
import matplotlib.pyplot as plt
from pulse2percept.datasets import load_perezfornos2012

data = load_perezfornos2012()
print(data)
```

## File description
- ```baseline_training.ipynb``` and ```baseline_evaluation.ipynb```: baseline model training and evalution. Code adapted from Avraham, David, et al. “Retinal Prosthetic Vision Simulation: Temporal Aspects.” Journal of Neural Engineering, vol. 18, no. 4, IOP Publishing, Aug. 2021, p. 0460d9, doi:10.1088/1741-2552/ac1b6c.
- ```exponential_cross_subject.ipynb```: Exponential model trained and evaluted using leave-one-subject-out cross-validation. 
- ```exponential_cross_stimulus.ipynb```: Exponential model trained and evaluted using leave-one-stimulus-condition-out cross-validation. 
- ```FFT_cross_subject.ipynb```: FFT model trained and evaluted using leave-one-subject-out cross-validation. 
- ```FFT_cross_stimulus.ipynb```: FFT model trained and evaluted using leave-one-stimulus-condition-out cross-validation. 
