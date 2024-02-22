kubectl apply -f "./jokes-app-mern/jokes-db/k8s"

kubectl apply -f "./jokes-app-mern/jokes-api/k8s"

kubectl get pod

kubectl logs <pod-name>

kubectl delete -f "./jokes-app-mern/jokes-api/k8s"

// update image and push
docker image build -t somnath8das/jokes-api:2.0 "./jokes-app-mern\jokes-api"

docker push somnath8das/jokes-api:2.0
