// need to enable kubernetes in docker

kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.7.0/aio/deploy/recommended.yaml

// run kubernetes server
kubectl proxy

// go to this link
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/#/login

kubectl apply -f Dashboard.yaml

// get the token and paste on link
kubectl -n kubernetes-dashboard create token admin-user

// create pod
kubectl apply -f "./simple-node-app/k8s/simpleapp-pod.yaml"

// see pod list
kubectl get pod

// create service
kubectl apply -f "./simple-node-app/k8s/simpleapp-service.yaml"

// see service list
kubectl get services

// apply deployment
kubectl apply -f "./simple-node-app/k8s/simpleapp-deployment.yaml"

// see pod list
kubectl get pod

// delete pod
kubectl delete pod <pod-name>

// delete service
kubectl delete service <service-name>
