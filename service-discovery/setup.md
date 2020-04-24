#Mysql setup
kubectl create -f mysql-database.yaml
#Logs
kubectl logs --follow pod/database
#Login into Mysql DB container
kubectl exec database -it -- mysql -u root -p
