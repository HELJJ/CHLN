# Collaborative Hypergraph Neural Network for Sequential Diagnosis Prediction

Codes for paper: *Collaborative Hypergraph Neural Network for Sequential Diagnosis Prediction*

## Requirements

pip install -r requirements.txt



## 1. Prepare the datasets



### (1) Download the MIMIC-III and MIMIC-IV datasets

The original datasets can be downloaded from the following URLs.

Go to [https://mimic.physionet.org/](https://mimic.physionet.org/gettingstarted/access/) for access. Once you have the authority for the dataset, download the dataset and extract the csv files to `data/mimic3/raw/` and `data/mimic4/raw/` in this project.

After the datasets are downloaded, please put each of them into a specified directory of the project.

## Folder Specification



- data/
  - mimic3
    - encoded
    - parsed
    - raw
    - standard
  - mimic4
    - encoded
    - parsed
    - raw
    - standard
  - params
    - mimic3
    - mimic4
  - icd9.txt
- raw
  - mimic3
    - ADMISSIONS.csv
    - DIAGNOSES_ICD.csv
    - PRESCRIPTIONS.csv
    - PATIENTS.csv
    - NOTEEVENTS.csv
  - mimic4
    - admissions.csv
    - diagnoses_ics.csv
    - prescriptions.csv
    - patient.csv
    - noteevents.csv

### (2) Preprocess datasets



````
python run_preprocess.py
````



## 2. Configuration

Please see `train.py` for detailed configurations.

## 3. Train model



You can train the model with the following command:

````
```bash
python train.py
```
````



## Acknowledgement



If this work is useful in your research, please cite our paper.
