# Kubernetes with Minikube

> This assumes that you have minikube installed and running.

## Applying the configs

The following are in order.

Apply the config

```bash
kubectl apply -f mongo-config.yaml
```

Apply the secret

```bash
kubectl apply -f mongo-secret.yaml
```

Apply the database

```bash
kubectl apply -f mongo.yaml
```

Apply the webapp

```bash
kubectl apply -f webapp.yaml
```

## Accessing the webapp

get the minikube ip

```bash
minikube ip
# or
kubectl get node -o wide
```
