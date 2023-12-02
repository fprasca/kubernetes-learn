# kubernetes-learn

Architecture of a Kubernetes cluster

![overview](images/k8_arch.drawio.png "k8 arch")

## Master Node
- API Server - what you (using kubectl) and other components of the control plane communicate with..
- Scheduler - this determines which worker node to create the pod in.
- Controller Manager - performs cluster-level functions, such as, replicating components, keeping track of worker nodes, handling node failures, etc.
- etcd - data store that persistently stores the cluster configuration.

## Woker Node
- Docker - container runtime, what runs your containers.
- Kubelet - talks to the API server and manages containers on its node.
- Kube-proxy - load-balances network traffic between application components.

## Tutorials
Video I watched to learn about k8s: [YouTube](https://youtu.be/7bA0gTroJjw?si=pjLvUtUuKT6ATTXX)

# Common kubectl commands

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