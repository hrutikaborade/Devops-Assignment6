# Devops-Assignment6
MYSQL node on Kubernetes using Kubernetes Artifacts 

**Question 
Problem Statement of the assignment: 

You need to install the MYSQL database on kubernetes using kubernetes artifact files i.e 

mysql-deployment.yaml 

mysql-configmap.yaml

mysql-service.yaml

mysql-secret.yaml 

**Answer

Steps : 

 1. Create a namespace : 
 
     kubectl create namespace demo
     
 2. Set the current namesapce to the one you created : 
    
     kubectl config set-context --current --namespace=demo
     
 3. Create secret  :
    
     kubectl create -f mysql-secret.yaml 

 4. Create configmap : 
    
     kubectl create -f mysql-configmap.yaml

 5. Create deployment for MySQL :
      
      kubectl create -f mysql-deployment.yaml 
      
      kubectl get pods --watch
     
 6. Create service for MySQL :
     
     kubectl create -f mysql-service.yaml
      


