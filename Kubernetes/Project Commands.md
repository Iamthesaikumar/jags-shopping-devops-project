Connect Kubectl to EKS.
aws eks update-kubeconfig --region us-east-2 --name Pixel

Deploy to Application.
kubectl apply -f deployment.yaml

view Application.
kubectl get deployment

View ReplicaSets.
kubectl get rs

View Pods.
kubectl get pods

Create Service.
kubectl apply -f service.yaml

View Service.
kubectl get svc

View Service Endpoints.
kubectl get endpoints

Check Rolling Update Status.
kubectl rollout status deployment/jags-deployment

View Rollout History.
kubectl rollout history deployment/jags-deployment

Rollback Deployment.
kubectl rollout undo deployment/jags-deployment
