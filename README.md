# Kubernetes Cheatsheet

### - Greate deployment
kubectl apply -f webserver-deployment.yml

### - Get deployments
kubectl get deployments

### - Get pods
kubectl get pods

### - Expose deployment
kubectl expose deployment webserver-deployment --type=LoadBalancer --port=80

### - Get services
kubectl get services

### - Get the URL for a service
minikube service webserver-deployment --url
