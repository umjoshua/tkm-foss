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
```
docker run -d --name jenkins -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v ~/.kube/config:/var/jenkins_home/.kube/config:ro -v /var/run/docker.sock:/var/run/docker.sock jenkins/jenkins:lts
```