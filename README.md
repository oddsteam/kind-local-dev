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

# Loading an Image Into Your Cluster
Docker images can be loaded into your cluster nodes with:
```
kind load docker-image my-custom-image-0 my-custom-image-1
```