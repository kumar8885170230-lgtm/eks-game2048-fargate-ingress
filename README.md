# AWS EKS Game 2048 Deployment

## Project Overview
Deployed the Game 2048 application on Amazon EKS using AWS Fargate, Kubernetes, the AWS Load Balancer Controller, and an Application Load Balancer.

## Architecture
User Browser -> AWS ALB -> Kubernetes Ingress -> Service -> Game 2048 Pods on Fargate

## Technologies Used
- Amazon EKS
- AWS Fargate
- Kubernetes
- AWS Load Balancer Controller
- Application Load Balancer
- Helm
- AWS CLI
- kubectl
- Git and GitHub

## Kubernetes Resources
- Namespace: game-2048
- Deployment: deployment-2048
- Service: service-2048
- Ingress: ingress-2048

## Configuration Files
- k8s/deployment.yaml
- k8s/service.yaml
- k8s/ingress.yaml

## Screenshots
See the screenshots folder for the application, ALB, and EKS cluster.

## Verification Commands
kubectl get pods -n game-2048
kubectl get svc -n game-2048
kubectl get ingress -n game-2048

## Troubleshooting
Investigated Kubernetes Ingress webhook availability, Service endpoints, and AWS load balancer connectivity.

## Cleanup
Delete unneeded AWS resources when finished to avoid ongoing charges.
