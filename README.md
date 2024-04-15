# Facial Liveness Verification System for KYC Solutions

Welcome to the Facial Liveness Verification System designed for KYC (Know Your Customer) services. This advanced system, crafted by the talented AI team at FinTechSys Company, leverages the MLflow framework to create a comprehensive MLOps project. Through the power of deep learning, it enables precise face liveness detection and seamless model deployment to web applications, enriched with additional AI functionalities like face tracking.

## System Overview

This documentation provides detailed instructions tailored for two distinct audiences:

### For Developers

Are you a developer eager to integrate this system into your KYC solution? Look no further! Part 1 of this documentation offers comprehensive instructions tailored specifically for you.

### For AI Developers

Seeking to enhance or retrain the existing model? Part 2 of this documentation is your gateway to contributing to our MLflow framework and Data Version Control (DVC), ensuring smooth model retraining and deployment across various systems.

## Framework Design

Our system is meticulously crafted to prioritize ease of use and flexibility. We've integrated MLOps principles at every stage of development, making model retraining a breeze. Simply modify the preprocessing data file and/or model preparation as needed. With our streamlined pipeline, training the model is as simple as executing a single command. This command automates data download, preprocessing, model building, training, and deployment, eliminating the need for manual intervention.

---

**Join us in revolutionizing KYC services with cutting-edge facial liveness verification!**




## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update the entity
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline 
7. Update the main.py
8. Update the dvc.yaml
9. app.py

# How to run?
### Part 1 - STEPS:

Clone the repository

```bash
https://github.com/fintechsys/liveness.git
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n liveness-env python=3.8 -y
```

```bash
conda activate liveness-env
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

```bash
# Run the following command
python setup.py install
```

```bash
# play the minio server to store image and video of user to it
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```






## Part 2 - MLOps and Data Version Control Steps:

For comprehensive documentation, refer to the [MLflow Documentation](https://mlflow.org/docs/latest/index.html).

### Command Line Instructions:

To launch the MLflow UI, use the following command:

```bash
mlflow ui


### dagshub
[dagshub](https://dagshub.com/)
MLFLOW_TRACKING_URI="YOUR_MLFLOW_TRACKING_URI"
MLFLOW_TRACKING_USERNAME="YOUR_DAGSHUB_USERNAME"
MLFLOW_TRACKING_PASSWORD="YOUR_DAGSHUB_PASSWORD"
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI="YOUR_MLFLOW_TRACKING_URI"
export MLFLOW_TRACKING_USERNAME="YOUR_DAGSHUB_USERNAME"
export MLFLOW_TRACKING_PASSWORD="YOUR_DAGSHUB_PASSWORD"

```


### DVC cmd

1. dvc init
2. dvc repro
3. dvc dag


## About MLflow & DVC

MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & taging your model


DVC 

 - Its very lite weight for POC only
 - lite weight expriements tracker
 - It can perform Orchestration (Creating Pipelines)


