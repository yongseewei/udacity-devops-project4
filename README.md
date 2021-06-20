[![CircleCI](https://circleci.com/gh/yongseewei/udacity-devops-project4/tree/main.svg?style=svg)](https://circleci.com/gh/yongseewei/udacity-devops-project4/tree/main)


## Project Summary

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

<!--### Project Tasks-->

<!--Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:-->
<!--* Test your project code using linting-->
<!--* Complete a Dockerfile to containerize this application-->
<!--* Deploy your containerized application using Docker and make a prediction-->
<!--* Improve the log statements in the source code for this application-->
<!--* Configure Kubernetes and create a Kubernetes cluster-->
<!--* Deploy a container using Kubernetes and make a prediction-->
<!--* Upload a complete Github repo with CircleCI to indicate that your code has been tested-->

<!--You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).-->

<!--**The final implementation of the project will showcase your abilities to operationalize production microservices.**-->

<!------->

## Setup the Environment

* Create a virtualenv and activate it
```python
python3 -m venv ~/.devops
source ~/.devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Making prediction
* Run `./make_prediction.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

### Files Listed
1. .circleci: circle ci config file
2. model_data: machine learning data
3. output_txt_files: consists of docker_out.txt and kubernetes_out.txt
4. app.py: python application file
5. Dockerfile: docker file
6. make_prediction.sh: script to make prediction
7. Makefile: make file (setup install lint test)
8. requirements.txt: python lib required for the project
9. run_docker.sh: script to build and run docker container
10. run_kubernetes.sh: script to run kubernetes
11. upload_docker.sh: scrip to upload docker to repo