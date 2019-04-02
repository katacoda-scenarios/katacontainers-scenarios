`minikube start \
   --feature-gates=RuntimeClass=true \
   --network-plugin=cni \
   --enable-default-cni \
   --container-runtime=cri-o `{{execute}}

```
git clone https://github.com/kata-containers/packaging.git
cd packaging/kata-deploy
kubectl apply -f kata-rbac.yaml
kubectl apply -f kata-deploy.yaml
```{{execute}}

`kubectl get ds -n kube-system`{{execute}}

`kubectl get pods -n kube-system -l name=kata-deploy`{{execute}}
