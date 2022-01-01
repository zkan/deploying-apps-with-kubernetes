# Deploying Apps with Kubernetes

## The Basics

```sh
kubectl create ns example
kubectl apply -f nginx/
```

## Kustomize

To generate rendered manifest files:

```sh
kubectl kustomize kustomize/environments/development/
```

To apply Kustomization:

```sh
kubectl create ns example
kubectl apply -k kustomize/environment/development/
```

## Helm

To render template:

```sh
helm template myapp helm
```

To install/upgrade Helm chart:

```sh
kubectl create ns example
helm upgrade --install myapp helm -n example
```

To uninstall Helm chart:

```sh
helm uninstall myapp -n example
```
