# kubectl Cheat Sheet

## Basic Commands:

| Command                                     | Description                                   |
|---------------------------------------------|-----------------------------------------------|
| `kubectl config get-contexts`               | List all available clusters (contexts)        |
| `kubectl config use-context <context-name>` | Switch to a different cluster                |
| `kubectl get nodes`                         | List all nodes in the cluster                 |
| `kubectl get namespaces`                    | List all namespaces in the cluster            |
| `kubectl get pods -n <namespace>`            | List all pods in a specific namespace         |
| `kubectl get services`                       | List all services in the cluster              |

## Cluster Management:

| Command                             | Description                                   |
|-------------------------------------|-----------------------------------------------|
| `kubectl create cluster ...`         | Create a new Kubernetes cluster (see specific provider documentation) |
| `kubectl config delete-context <context-name>` | Delete a cluster context from `kubeconfig`   |
| `kubectl delete pod <pod-name>`      | Delete a pod                                 |
| `kubectl delete deployment <deployment-name>` | Delete a deployment                    |

## Restart Pods in Namespace:

| Command                                          | Description                                   |
|--------------------------------------------------|-----------------------------------------------|
| `kubectl delete pods --all -n <namespace>`        | Delete all pods in a specific namespace       |
| `kubectl rollout restart deployment -n <namespace>` | Restart all pods in a deployment in a namespace |

Note: Replace `<context-name>`, `<namespace>`, `<pod-name>`, `<deployment-name>` with your actual values.
