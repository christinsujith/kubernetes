# kubernetes

# Deployment
kubectl create -f webserviceDeployment.yaml
# List running deployment
kubectl get deployments
# List Running Replica set
kubectl get rs
# List Running Pods
kubectl get pods
# Expose Deployment
kubectl expose deployment nginx-deployment --type=NodePort
# Get exposed service
kubectl get service
# Get deployment url
minikube service nginx-deployment --url


