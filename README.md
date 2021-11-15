# kubernetes-falco

## quickly start
```
helm repo add falcosecurity https://falcosecurity.github.io/charts
helm repo update

# create namespace
kubectl create ns falco


helm install falco falcosecurity/falco -n falco
```
