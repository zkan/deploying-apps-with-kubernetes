# Deploying Apps with Kubernetes

## The Basics

```sh
kubectl apply -f nginx/
```

## Kustomize

To generate rendered manifest files:

```sh
kubectl kustomize kustomize/environments/development/
```

To apply Kustomization:

```sh
kubectl apply -k kustomize/environment/development/
```
