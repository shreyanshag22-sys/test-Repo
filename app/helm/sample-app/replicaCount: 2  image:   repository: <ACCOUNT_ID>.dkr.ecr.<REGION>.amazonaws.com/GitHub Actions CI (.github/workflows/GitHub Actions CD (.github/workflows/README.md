# Sample Flask App on Amazon EKS

## Build locally

```bash
docker build -t sample-app ./app
```

Run locally:

```bash
docker run -p 5000:5000 sample-app
```

Deploy:

```bash
helm upgrade --install sample-app ./helm/sample-app
```

Check:

```bash
kubectl get pods

kubectl get svc
```
