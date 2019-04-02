`ps -ef | fgrep qemu-system`{{execute}}

`uname -a`{{execute}}

`export KATAPOD=$(kubectl get pods -l run=php-apache-kata-qemu -o jsonpath="{.items[0].metadata.name}")`{{execute}}

`kubectl exec -ti $KATAPOD bash`{{execute}}

`uname -a`{{execute}}

**Linux php-apache-kata-qemu-59b9b58955-c6zmr 4.4.0-141-generic #167-Ubuntu SMP Wed Dec 5 10:40:15 UTC 2018 x86_64 GNU/Linux**

