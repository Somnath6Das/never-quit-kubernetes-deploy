kubectl apply -f "./jokes-app-mern/jokes-db/k8s"

kubectl apply -f "./jokes-app-mern/jokes-api/k8s"

kubectl get pod

kubectl logs <pod-name>

kubectl delete -f "./jokes-app-mern/jokes-api/k8s"
