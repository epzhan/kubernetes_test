# start the local k8s
```
minikube config set driver hyperv \
minikube start \
minikube stop \
minikube dashboard \

minikube image \
minikube image load coreweb:1.0 \
minikube image rm coreweb:1.0 \
```

# apply the k8s pod config
```
kubectl apply -f mongo-config.yaml \
kubectl apply -f mongo-secret.yaml \
kubectl apply -f mongo.yaml \
kubectl apply -f webapp.yaml \
```
# interating with k8s cluster
```
kubectl get all \
kubectl get configmap \
kubectl get secret \
kubectl get pod \
kubectl describe service webapp-service \
kubectl logs <podName> -f \
```

# access to web application address
```
minikube ip \
minikube service webapp-service \
minikube service --all \
kubectl get svc \
kubectl get node -o wide \
```

## references
https://minikube.sigs.k8s.io/docs/handbook/accessing/ \
https://gitlab.com/nanuchi/k8s-in-1-hour
