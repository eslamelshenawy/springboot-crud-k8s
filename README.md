# springboot-crud-k8s
Run &amp; Deploy Spring Boot CRUD Application With MySQL on K8S

```bash
minikube start
```

```bash
eval $(minikube docker-env)
```
```bash
kubectl apply -f db-deployment.yaml
```
```bash
kubectl apply -f mysql-secrets.yaml
```
```bash
kubectl apply -f mysql-configMap.yaml
```
```bash
kubectl get deployments
```
```bash
kubectl get pods
```
```bash
kubectl logs mysql-76c6bf8f88-fvtpb
```
```bash
kubectl describe pod mysql-76c6bf8f88-2w9b7
```
```bash
kubectl exec -it mysql-76c6bf8f88-5kwhc /bin/bash
```
```bash
mysql -h mysql -u root -p  # username root #password root
```
```bash
show databases ;  # use javatechie // show tables;
```
```bash
docker build -t springboot-crud-k8s:1.0 .
```
```bash
kubectl apply -f app-deployment.yaml
```
```bash
kubectl get svc
```
```bash
minikube ip # ip:32111  //like 8080:32111/TCP .... from kubectl get svc
```
```bash
minikube dashboard 
```
