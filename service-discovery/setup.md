# Mysql setup
kubectl create -f mysql-database.yaml
# Logs
kubectl logs --follow pod/database
# Login into Mysql DB container
kubectl exec database -it -- mysql -u root -p
# Create DB service
kubectl create -f database-service.yaml
# List all services
kubectl get services

# Create node js web
kubectl create -f nodejs-web.yaml

# Create node js web service
kubectl create -f nodejs-web-service.yaml