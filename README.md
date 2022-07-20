# Chart Source
https://bitnami.com/stack/jenkins/helm

## Installation command
helm install [RELEASE_NAME] bitnami/jenkins
helm install jenkins -f values.yaml bitnami/jenkins

## Minikube
minikube addons enable ingress
minikube tunnel
