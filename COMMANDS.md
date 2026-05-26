After installing minikube, which is local software to test kubernetes in your system

How to start minikube

```
minikube start
minikube stop
```

```
kubectl get namespaces
```

Create namespaces

```
kubectl apply -f namespace.yaml
```

```
kubectl delete -f namespace.yaml
```

```
kubectl apply -f deployment.yaml
```

```
kubectl get deployments -n development
```

```
kubectl get pods -n development
```

```
kubectl delete pod <pod_name> -n development
```

```
kubectl describe pod <pod_name> -n development
```

```
kubectl get pods -n development -o wide
```

```
kubectl apply -f busybox.yaml 
```

```
kubectl get pods
```

```
kubectl exec -it busybox-pod-name -- /bin/sh

wget 172.17.0.05:3000 (port methoned in deployement.yml)

cat index.html

exit
```

```
kubectl logs <pod_name> -n development
```