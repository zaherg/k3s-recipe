# Guide

1. Create Namespace

```shell
kubectl create namespace redis-server
```

2. Create Persistent storage PVC

```shell
kubectl apply -f pvc.yml
```

3. Create Deployment

```shell
kubectl apply -f deployment.yml
```

You can check for the deployment process by checking the pods

```shell
kubectl get pods -n redis-server
```

4. Create Service

```shell
kubectl apply -f service.yml
```
 You can check if everything is okay by running

 ```shell
 kubectl get svc -n redis-server
 ```