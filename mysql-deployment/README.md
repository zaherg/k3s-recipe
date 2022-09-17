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
kubectl apply -f deployment.yml
```

You can check for the deployment process by checking the pods

```shell
kubectl get pods -n mysql-server
```

5. Create Service

```shell
kubectl apply -f service.yml
```

You can check if everything is okay by running

```shell
kubectl get svc -n mysql-server
```