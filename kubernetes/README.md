# Kubernized Minetrack

To use the kubernized version, first check for the correct image specified in the `minetrack-deployment.yaml` manifest. Currently the public Docker Hub is configured, change it to fit your needs.

Other than that to note: The tracked data is currently not persisted, that means on restart all data will get lost.

# How to use

Simply connect to your cluster, so that `kubectl` works properly.

Then use `kubectl apply -k .` to deploy it onto your cluster. To access it from outside, create a NodePort or an appropiate Ingress afterwards. 