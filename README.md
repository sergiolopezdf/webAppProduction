# WebApp Deployment: an example on how to deploy apps based on Docker, Docker Compose and Kubernetes

In this repository, you will be able to find examples on how to deploy this app:

https://github.com/sergiolopezdf/WebApp_TFG

Feel free to try it in your own deployments.

Although each branch contains a folder called 'containers', all containers are downloaded from hub.docker.com. It includes the Dockerfiles and the necessary items to build the containers.

## Requisites
	* Docker
	* Docker Compose
	* Kubectl
	* Docker Hub Account
	* Either minikube or an account on Google Cloud

## Branches

### DockerCompose
It contains the docker-compose.yaml. The way of using it is by running `sudo docker-compose up -d` within the folder you have the file. It will automatically build the containers.

### Kubernetes / KubernetesMultiPod
Examples on how to deploy on either Minikube or Google Cloud based on NodePort services. 

The command to run any of them is `kubectl create -f FILE_NAME.yaml`. 

Make sure the last deployment you run is WebAPP. You will need to change manually the both URL ENVIRONMENT VARIABLES and the PORT ENVIRONMENT VARIABLES in its deployment file.

### CloudDeployment
It is the same as the previous branch but it works with Load Balancer type of services.
