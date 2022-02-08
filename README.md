# kubernetes-postgresql

```
minikube mount .:/mnt/data
```

```
kubectl create -f postgres-configmap.yaml 
```

```
kubectl create -f postgres-storage.yaml 
```

```
kubectl create -f postgres-deployment.yaml 
```

```
kubectl create -f postgres-service.yaml 
```

```
kubectl get svc postgres
NAME       TYPE       CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
postgres   NodePort   10.107.71.253   <none>        5432:31070/TCP   5m
```

```
psql -h localhost -U postgresadmin1 --password -p 31070 postgresdb
```
