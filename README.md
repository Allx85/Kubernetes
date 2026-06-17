# Kubernetes

## Installation
[Kubernetes-install](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)

kind create cluster --name labb --config cluster.yaml <-- skapa ett cluster med yaml

kubectl create deployment nginx --image=nginx --replicas=2  <-- skapar 2 pods som kör nginx

kubectl apply -f filnamn <-- deployment med *.yaml*

curl -s 127.0.0.1:32650 <-- testa

kubectl get pods -o wide <-- kollar vilken nod pods ligger på

kubectl autoscale deployment bar-app --min=1 --max=5 --cpu=50% <-- sätter autoscaling på bar-app från minst 1 till max 5 och det sker vid 50% CPU användning

kubectl get hpa <-- visar inställningar för Horizontal Pod Autoscaler