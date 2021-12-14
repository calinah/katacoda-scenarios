# Let's deploy an app for Step 2

Using the k3s CLI, it's possible to access `kubectl` and inspect the cluster configuration.

`k3s kubectl cluster-info`{{execute T2}}

`k3s kubectl get node`{{execute T2}}

View the pods running with the command:

`k3s kubectl get pods --all-namespaces`{{execute T2}}

To save time, alias k3s kubectl to k.

`alias k="k3s kubectl"`{{execute T2}}

You can now use

`k get pods --all-namespaces`{{execute T2}}

Deploy a simple app using:

`k apply -f /usr/local/bin/service.yaml`{{execute T2}}