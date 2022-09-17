# Guide

1. Create Namespace

```shell
kubectl create namespace rethinkdb-server
```

2. Create Persistent storage PVC

```shell
kubectl apply -f pvc.yml
```

3. Create Deployment

```shell
kubectl apply -f .
```


You can check if everything is okay by running

 ```shell
 kubectl get svc -n rethinkdb-server
 ```