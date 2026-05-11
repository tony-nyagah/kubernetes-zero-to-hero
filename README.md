## Kubernetes Zero to Hero
Notes and code made while going through the Kubernetes Zero to Hero video: https://www.youtube.com/watch?v=MTHGoGUFpvE

### Creating a Pod
To create a pod, you can use a manifest file for example:
```
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
spec:
  containers:
  - name: my-container
    image: my-app:latest
    ports:
    - containerPort: 80
```

We run it using `kubectl apply -f my-pod.yaml`
