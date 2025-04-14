# Useful Kubernetes Commands for This Project

## Start Minikube

minikube start

## View Cluster Info

kubectl cluster-info

## Apply Deployment

kubectl apply -f k8s/deployment.yaml

## Apply Service

kubectl apply -f k8s/service.yaml

## Check Pods

kubectl get pods

## Check Services

kubectl get svc

## Describe Pod

kubectl describe pod <pod-name>

## Scale Deployment

kubectl scale deployment nginx-deployment --replicas=3

## Open NodePort Service in Browser

minikube service nginx-service

## Delete All Resources

kubectl delete -f k8s/
