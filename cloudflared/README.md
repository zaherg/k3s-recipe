# Guide

1. Create Namespace

```shell
kubectl create namespace cloudflare-server
```

2. copy `deployment.yml.dist` to a new file called `deployment.yml` and add your own token

3. Create Persistent storage PVC

```shell
kubectl apply -f .
```

You can check if everything is okay by running

 ```shell
 kubectl get svc -n cloudflare-server
 ```