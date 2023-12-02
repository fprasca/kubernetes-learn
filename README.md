# kubernetes-learn

Architecture of a Kubernetes cluster

![overview](images/k8_arch.drawio.png "k8 arch")

# common kubectl commands

- kubectl cluster-info
- kubectl describe pods
- kubectl describe services
- kubectl get nodes
- kubectl get deployments
- kubectl get pods
- kubectl get pods -o wide
- kubectl get services
- kubectl apply -f example-service.yml
- kubectl run mytestpod --image=thenetworkchuck/nccoffee:pourover --port=80