# kubernetes-p
## Lets take a look at kubernetes commands 
kubectl get pods --all-namespaces

kubectl get svc --all-namespaces

kubectl get pv,pvc

kubectl get nodes -o wide

kubectl describe po pod-name
  
kubectl describe svc service-name

kubectl describe serviceaccount service-account-name -n namespaces # without -n namespace option will take default namespace

## Expose Service to nodeport

kubectl expose pod/tomcat --name=tomcat-service --type=NodePort --port 8080

kubectl expose deployment/httpd-deployment --name=httpd-service --type=NodePort  --port 80

## Create a pod/deployment usuing a file

kubectl create -f test-mutipod-deployment.yaml

## Display all modules of a Namespace

kubectl get all -n kube-system

kubectl get all -n default

kubectl get all -n (name-of-the-namespace)

## List all name spaces

kubectl get sa --all-namespaces

## Edit a resource in kubernetes

kubectl edit pod kubernetes-dashboard-7b544877d5-f5xrv -n kubernetes-dashboard

kubectl edit svc kubernetes-dashboard -n kubernetes-dashboard

SYNTAX: kubectl edit pod or svc or deployment (name of the pod/svc/deploy) -n (name-of-the-namespace)
