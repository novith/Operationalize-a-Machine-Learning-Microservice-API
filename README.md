[![<novith>](https://circleci.com/gh/novith/Operationalize-a-Machine-Learning-Microservice-API.svg?style=svg)](https://circleci.com/gh/novith/Operationalize-a-Machine-Learning-Microservice-API)

## Operationalize-a-Machine-Learning-Microservice-API
This repository contains the Udacity assignment, Operationalize a Machine Learning Microservice API. The Project consists of deploying a containerized Python flask application to make predictions about Boston housing prices through API calls. It uses a a pre-trained, sklearn model tha pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on the data source site. 

## Environment requirements

* Docker
* hadolint
* Kubernetes and Minikube

## Setup the Environment

* Create a virtualenv and activate it (Windows 10 instructions)

	virtualenv -py python3 dir

	dir\Scripts\activate
    
* Run `make install` to install the necessary dependencies

### Files 
* config.yml: CircleCI configuration file
* Dockerfile: Dockerfile for building the image
* Makefile: Environment setup instructions and lint tests
* app.py: Python app that predicts housing prices through API calls
* make_prediction.sh: Send a request to the Python flask app to get a prediction
* run_docker.sh: Shell script to run and build a docker image, locally
* run_kubernetes.sh: file to run the app in kubernetes
* upload_docker.sh: file to upload the image to docker

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

