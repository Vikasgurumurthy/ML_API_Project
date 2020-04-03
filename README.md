[![CircleCI](https://circleci.com/gh/circleci/circleci-docs/tree/teesloane-patch-5.svg?style=svg)](https://app.circleci.com/pipelines/github/Vikasgurumurthy/ML_API_Project)

 # Operationalize a Machine Learning Microservice-API
The goal of this project is to opertionalise pretained ML model using Docker to contanierise it and Orchestration of docker using Kubernetes.

### Install 
Containerization : Docker<br />
Orchestration : Kubernates<br />
Circle CI<br />
Virtualbox<br />

### Instructions on how to run the Python scripts and web app
To run Container <br />
./run_docker.sh<br />
Make a Prediction<br />
./make_prediction.sh<br />
Upload image to Dockerhub<br />
./upload_docker.sh<br />
To start Kube cluster<br />
minikube start<br />
Create pod and deploy application<br />
./run_kubernetes.sh<br />
Delete Cluster<br />
minikube delete<br />

### Files in repository
config.yml: CircleCI configuration file for running the tests and lynting files<br />
app.py: Python flask app that serves out predictions (inference) about housing prices through API calls<br />
Dockerfile: Code for building Docker Image<br />
make_prediction.sh: Send a request to the Python flask app to get a prediction, for localhost<br />
make_prediction2.sh: Send a request to the Python flask app to get a prediction, for minikube kubernetes<br />
Makefile: Instructions for environment setup and lint tests<br />
run_docker.sh: Code to run docker locally<br />
run_kubernetes.sh: Code to run the app in kubernetes<br />
upload_docker.sh: Code to upload the image to dockerhub<br />
