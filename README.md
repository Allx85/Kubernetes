# Kubernetes

## Installation
[Kubernetes-install](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)

kind create cluster --name labb --config cluster.yaml <-- skapa ett cluster med yaml

kubectl create deployment nginx --image=nginx --replicas=2  <-- skapar 2 pods som kör nginx

kubectl apply -f filnamn <-- deployment med *.yaml*

curl -s 127.0.0.1:32650 <-- testa

kubectl get pods -o wide <-- kollar vilken nod pods ligger på