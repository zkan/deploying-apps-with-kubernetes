# Deploying Apps with Kubernetes

## The Basics

```sh
kubectl apply -f nginx/
```

## Kustomize

```sh
kubectl kustomize kustomize/environments/development/
```

or

```sh
kubectl apply -k kustomize/environment/development/
```
