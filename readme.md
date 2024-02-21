// need to enable kubernetes in docker

kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.7.0/aio/deploy/recommended.yaml

// run kubernetes server

kubectl proxy

// go to this link

http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/#/login

// apply dashboard

kubectl apply -f Dashboard.yaml

// get the token and paste on link

kubectl -n kubernetes-dashboard create token admin-user