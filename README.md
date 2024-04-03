# MLflow-Basic-Operation


## For Dagshub

MLFLOW_TRACKING_URI=https://dagshub.com/simonmontt/MLflow-Basic-Operation.mlflow \
MLFLOW_TRACKING_USERNAME=simonmontt \
MLFLOW_TRACKING_PASSWORD=b6cd9be87f377a371f06a721028cc2bf17be5e4c \
python script.py


## Export to my environment

``` bash 

export MLFLOW_TRACKING_URI=https://dagshub.com/simonmontt/MLflow-Basic-Operation.mlflow

export MLFLOW_TRACKING_USERNAME=simonmontt 

export MLFLOW_TRACKING_PASSWORD=b6cd9be87f377a371f06a721028cc2bf17be5e4c

``` bash


sudo apt update

sudo apt install python3-pip

sudo pip3 install pipenv

sudo pip3 install virtualenv

mkdir mlflow

cd mlflow

pipenv install mlflow

pipenv install awscli

pipenv install boto3

pipenv shell


## Then set aws credentials
aws configure


#Finally 
mlflow server -h 0.0.0.0 --default-artifact-root s3://mlflowbuc23

#open Public IPv4 DNS to the port 5000


#set uri in your local terminal and in your code 
export MLFLOW_TRACKING_URI=http://ec2-54-82-233-30.compute-1.amazonaws.com:5000/