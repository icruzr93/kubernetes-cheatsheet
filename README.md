# Kubernetes Cheatsheet

### Create deployment
```sh
kubectl apply -f webserver-deployment.yml
```

### Get deployments
```sh
kubectl get deployments
```

### Get pods
```sh
kubectl get pods
```

### Expose deployment
```sh
kubectl expose deployment webserver-deployment --type=LoadBalancer --port=80
```

### Get services
```sh
kubectl get services
```

### Get the URL for a service
```sh
minikube service webserver-deployment --url
```

### Scale a replicaset named 'foo' to 3.
```sh
kubectl scale --replicas=3 rs/foo
```

### Scale a resource identified by type and name specified in "foo.yaml" to 3.
```sh
kubectl scale --replicas=3 -f foo.yaml
```
### Get All
```sh
kubectl get all
```

### Delete deployment And Service
```sh
kubectl delete deploy/simple-deployment service/webserver-deploymen
```
