` curl https://raw.githubusercontent.com/kubernetes/node-api/master/manifests/runtimeclass_crd.yaml > runtimeclass_crd.yaml`{{execute}}

`kubectl apply -f runtimeclass_crd.yaml`{{execute}}


`git clone https://github.com/clearlinux/cloud-native-setup.git`{{execute}}

`cd cloud-native-setup/clr-k8s-examples`{{execute}}

`kubectl apply -f 8-kata/kata-qemu-runtimeClass.yaml`{{execute}}
