# Core Concepts


### Kube API Server 

### Kube-Controller Manager
- Node monitor period is 5seconds
- 40 seconds for grace period

### Kube Schedular

### Kubelet
- Need to install Kublet as process manually, unlike other parts 

#### Kube Proxy
- Every pod can interact with other pods 
- kube proxy is a process , who looks for any service created and suitable rules/ routing to forward traffic
- kube proxy runs as daemonset in kube adm , while it installed as serice if done seprately 

## Kubernetes resource

Pod, Deployment

**Replication Controller** vs **Replica Set** 
Selector (in form of matchLablels) is key difference two. As ReplicaSet can use existening pod using matchLablels

Pod Capacity in a Node
kubectl get node <node_name> -ojsonpath='{.status.capacity.pods}'
