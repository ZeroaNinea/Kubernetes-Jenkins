# Kubernetes Manifests for Jenkins Deployment

Refer https://devopscube.com/setup-jenkins-on-kubernetes-cluster/ for step by step process to use these manifests.

## Get the Password

```bash
kubectl get pods -n devops-tools
kubectl logs POD_NAME -n devops-tools

```
