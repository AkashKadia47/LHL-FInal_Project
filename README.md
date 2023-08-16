# PotatoAI : Disease Detection for Healthy Harvests 

This deep learning project will utilize CNN to identify diseases in potato plants. The model will analyze images to provide accurate disease detection, aiding in better crop management.

## Data

Downloaded the data from [kaggle](https://www.kaggle.com/arjuntejaswi/plant-village).

## Prerequisites
### Setup for Python:

1. Install Python ([Setup instructions](https://wiki.python.org/moin/BeginnersGuide))

2. Install Python packages

```
pip3 install -r training/requirements.txt
pip3 install -r api/requirements.txt
```

3. Install Tensorflow Serving ([Setup instructions](https://www.tensorflow.org/tfx/serving/setup))

## Model testing
- local machine
1. run api\main.py
2. postman:
    - post request url: http://localhost:8000/predict
    - BODY -> form-data -> Key: file ; Value: use any images from the saved_models

## File Organization and Contents

## api
1. requirement.txt :
Run this to install all the requird liberaries.
2. main.py : code for API using Fast API.

### data
1. Early Blight: 1000 photos of potato leaves have Early Blight desease.
2. Healthy: 251 photos of potato leaves are healthy.
3. Late Blight: 1000 photos of potato leaves have Late Blight desease

### gcp
1. requirement.txt :
Run this to install all the requird liberaries.
2. main.py : code for GCP deploy.

### Presentation
PotatoAI.pptx : Presentation of the project

### saved_models
1. Numbered Folder are model version
2. latest_potato_model.h5: latest model deployed on the GCP.

### test_images_from_internet
images to test on postman downloaded from the internet

### training.ipynb
Data preprocessing and model building

## Authors

* **Akash Kadia** - *Entire Project* - [AkashKadia47](https://github.com/AkashKadia47)

