# Kubernetes Manifests for Jenkins Deployment

Refer https://devopscube.com/setup-jenkins-on-kubernetes-cluster/ for step by step process to use these manifests.

## Get the Password

```bash
kubectl get pods -n devops-tools
kubectl logs POD_NAME -n devops-tools

```

Apply all the files:

```bash
kubectl apply -f namespace.yaml
kubectl apply -f serviceAccount.yaml
kubectl apply -f volume.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f jenkins-ingress.yaml

```

Delete all the file:

```bash
kubectl delete -f namespace.yaml
kubectl delete -f serviceAccount.yaml
kubectl delete -f volume.yaml
kubectl delete -f deployment.yaml
kubectl delete -f service.yaml
kubectl delete -f jenkins-ingress.yaml

```
