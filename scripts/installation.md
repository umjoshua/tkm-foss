# Environment Setup
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
