

# Privacy-Onion-Effect

This repository contains the backbone core of the paper "FT-PrivacyScore: Personalized Privacy Scoring Service for Machine Learning Participation"


## Installation

To install the necessary environment for running this implementation, use the following command:

```bash
conda env create -f cifar/environment.yaml
```

## Pre-Configuration

You need to adjust the absolute paths in the following files to your specific absolute paths:

- `cifar/MIA/configs/config_attack.yaml`
- `cifar/MIA/scripts/static.py`
- `cifar/MIA/scripts/privacy_score.py`

## Run Experiment

1. **Generate Experiment Models**: Run the `cifar/train_cifar.sh` script to generate the experiment models.

2. **Generate Results**:
   - Navigate to the `MIA` directory to ensure the data addresses are correct.
   - Execute the `./run_all.py` script to:
     - Generate shadow models.
     - Obtain observations from the shadow datasets.
     - Compute Gaussian distribution parameters.
     - Generate attack results on the experiment models.
     - Produce privacy scores for each sample.




