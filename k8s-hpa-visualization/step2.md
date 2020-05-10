first we set up our visualization stack

clone `kube-prometheus` repository

`git clone https://github.com/coreos/kube-prometheus.git`{{execute}}

next, we go into the repository and spawn the monitoring namespaces and containers.

**Be sure to wait each command is complteted and all containers are running before moving to the next**

`kubectl create -f manifests/setup`{{execute}}

`kubectl create -f manifests/`{{execute}}

to check for the status of the containers use
`kubectl get pods --namespace=monitoring`{{execute}}