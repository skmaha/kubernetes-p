# kubernetes-p
# Lets take a look at kubernetes commands 
kubectl get pods --all-namespaces

kubectl get svc --all-namespaces

kubectl get pv,pvc

kubectl get nodes -o wide

kubectl describe po pod-name
  
kubectl describe svc service-name

kubectl describe serviceaccount service-account-name -n namespaces # without -n namespace option will take default namespace
