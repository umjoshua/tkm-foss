# Environment  - Windows
## Installing Docker desktop
```
winget install -e --id Docker.DockerDesktop
```

## Install Minikube
```
winget install -e --id Kubernetes.minikube
```

## Install kubectl
```
winget install -e --id Kubernetes.kubectl
```

## Starting minikube
```
minikube start
```

# CI / CD Setup
## Running Jenkins

1. Run the jenkins docker container
```
docker run -d --name jenkins -p 8080:8080 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```
# Environment  - Linux

1. Docker installation
Reference: https://snapcraft.io/docker

```
sudo snap install docker

sudo snap install docker

sudo addgroup --system docker

sudo adduser $USER docker

newgrp docker

sudo snap disable docker

sudo snap enable docker
```

2. Minikube installation
```
Minikube installation
Reference: https://snapcraft.io/minikube

sudo snap install minikube

minikube start

minikube stop

kubectl
Ref: https://snapcraft.io/kubectl
sudo snap install kubectl --classic
```