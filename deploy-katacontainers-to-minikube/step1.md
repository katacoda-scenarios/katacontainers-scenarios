`add-apt-repository -y ppa:projectatomic/ppa`{{execute}}

```
apt-get update
apt-get install -y cri-o-1.11
```{{execute}}

`minikube start \
   --feature-gates=RuntimeClass=true \
   --network-plugin=cni \
   --enable-default-cni \
   --container-runtime=cri-o `{{execute}}

