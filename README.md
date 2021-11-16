# kubernetes-falco

## quickly start
```
helm repo add falcosecurity https://falcosecurity.github.io/charts
helm repo update

# create namespace
kubectl create ns falco


helm install falco falcosecurity/falco -n falco
```
完整內容[falco charts](https://github.com/falcosecurity/charts)

test for falco
```
kubectl create ns ping
kubectl create -f mysql-deployment.yaml -n ping
kubectl create -f mysql-service.yaml -n ping
kubectl create -f ping-deployment.yaml -n ping
kubectl create -f ping-service.yaml -n ping
kubectl create -f client-deployment.yaml -n ping
```


