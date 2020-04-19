# kubernetes

# Deployment
kubectl create -f webserviceDeployment.yaml
# List running deployment
kubectl get deployments
# List Running Replica set
kubectl get rs
# List Running Pods
kubectl get pods
# List Running Pods with labels
kubectl get pods --show-labels
# Expose Deployment
kubectl expose deployment nginx-deployment --type=NodePort
# Get exposed service
kubectl get service
# Get deployment url
minikube service nginx-deployment --url
# Update image
kubectl set image deployment nginx-deployment nginx=christinsujith/latestnginx
# Rollout image
kubectl rollout status deployment nginx-deployment
# Rollout History
kubectl rollout history deployment nginx-deployment
# Rollback changes
kubectl rollout undo deployment nginx-deployment
# Edit deployment
kubectl edit deployment nginx-deployment
# Add Label
kubectl label nodes minikube disktype=ssd


