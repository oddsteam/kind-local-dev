# kind-local-dev

สรา้ง Cluster
```
kind create cluster
```

```
kind create cluster --name kind-2
```
```
kind create cluster --config kind-multi-node-config.yaml --name kind-multi-node

kind delete cluster --name kind-multi-node
```

```
kind create cluster --config kind-portmapping.yaml --name kind-portmap  
```
```
kubectl apply -f httpbin-deployment.yaml
```
```
  kubectl create namespace ingress-nginx
```
```
kind create cluster --config kind-ingress.yaml --name kind-ingress

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.10.0/deploy/static/provider/kind/deploy.yaml
```
# Loading an Image Into Your Cluster
Docker images can be loaded into your cluster nodes with:
```
kind load docker-image my-custom-image-0 my-custom-image-1
```


```
kubectl port-forward service/web-server-service 8080:80
```