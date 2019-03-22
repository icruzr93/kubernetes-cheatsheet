# Kubernetes Cheatsheet

### Create deployment
kubectl apply -f webserver-deployment.yml

### Get deployments
kubectl get deployments

### Get pods
kubectl get pods

### Expose deployment
kubectl expose deployment webserver-deployment --type=LoadBalancer --port=80

### Get services
kubectl get services

### Get the URL for a service
minikube service webserver-deployment --url

### Scale a replicaset named 'foo' to 3.
kubectl scale --replicas=3 rs/foo

### Scale a resource identified by type and name specified in "foo.yaml" to 3.
kubectl scale --replicas=3 -f foo.yaml

### Get All
kubectl get all

### Delete deployment And Service
kubectl delete deploy/simple-deployment service/webserver-deploymen
