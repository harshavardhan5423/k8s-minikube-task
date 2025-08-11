# Task 5: Build a Kubernetes Cluster Locally with Minikube

## Objective
Deploy and manage applications in Kubernetes using Minikube.

## Tools Used
- **Minikube**
- **kubectl**
- **Docker**

## Steps Performed
1. **Installed Minikube** and started the cluster:
   ```bash
   minikube start
Created deployment.yaml to deploy an Nginx application.
Applied the deployment:
kubectl apply -f deployment.yaml
Created service.yaml to expose the deployment.
Applied the service:
kubectl apply -f service.yaml
Verified pods and services:
kubectl get pods
kubectl get svc
Described pod and service details:
kubectl describe pod <pod-name>
kubectl describe svc <service-name>
Scaled the deployment to 3 replicas:
kubectl scale deployment nginx-deployment --replicas=3
kubectl get pods
Saved outputs/screenshots:
screenshots/pods-list.txt
screenshots/service-details.txt
pod-details.txt
deployment.yaml
service.yaml
Deliverables
deployment.yaml – Deployment configuration.
service.yaml – Service configuration.
Output text files with pod and service details.
This README.md.
Notes
Ensure Minikube is running before applying manifests.
Use minikube service <service-name> to access the application locally.
