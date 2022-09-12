# k8s Study

This was a project to understand about k8s and how it works.

# k8s Commands

List of commands for k8s management:

# Pods
```
$ kubectl get pods
$ kubectl get pods --all-namespaces
$ kubectl get pod POD_NAME -o wide
$ kubectl get pod POD_NAME -o yaml
```

# Create Deployments

```
$ kubectl run POD_NAME --image=POD_NAME --record
```

# Scaling

```
$ kubectl scale deployment/POD_NAME --replicas=N
```

# Services

```
$ kubectl get services
$ kubectl expose deployment/POD_NAME --port=2001 --type=NodePort
```

# Volumes

```
$ kubectl get pv
$ kubectl get pvc
```

# Secrets

```
$ kubectl get secrets
$ kubectl create secret SECRET_NAME --help
$ kubectl create secret SECRET_NAME postgresql --from-literal=password=root
$ kubectl get secrets mysql -o yaml
```

# Troubleshooting

```
$ kubectl describe
$ kubectl get nodes --show-labels
$ kubectl get events
$ kubectl exec
$ kubectl logs
```