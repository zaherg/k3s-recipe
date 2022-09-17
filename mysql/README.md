# Guide

1. Create Namespace

```shell
kubectl create namespace mysql-server
```

2. Create Persistent storage PVC

```shell
kubectl apply -f pvc.yml
```

3. Create the configuration

```shell
kubectl create configmap mysql-config --from-file=main-config=my-custom.cnf -n mysql-server
```

4. Create Deployment

```shell
kubectl apply -f .
```

You can check if everything is okay by running

```shell
kubectl get svc -n mysql-server
```