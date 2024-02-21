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
kubectl delete -f "./simple-node-app/k8s/simpleapp-pod.yaml"

// delete service

kubectl delete service <service-name>
