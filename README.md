# Kubernetes-helm

### Get current context
```
 kubectl get current-context
```

### Add bitnami repo helm
```
helm repo add bitnami https://charts.bitnami.com/bitnami
```

### Get all the repo of bitnami
```
helm search repo bitnami
```

### Grep specific repo
```
helm search repo bitnami | grep nginx
```


### install nginx using helm
```
helm install nginxv1 bitnami/nginx
```

### install prometheus using helm
```
helm install prometheusv1 bitnami/prometheus
```

### Add eks repo with helm
```
helm repo add eks https://aws.github.io/eks-charts
```

### Update repo 
```
helm repo update eks
```

### Get list helm
```
helm list
```

### uninstall specific installation
```
 helm uninstall nginxv1
```
- Uninstalling specific installation also deletes pods

### Create charts
```
helm create payments
helm create shipping
```
### files info
- Deployment.yaml
    - Contains deployment related configuration
- values.yaml
    - to provide variables to any yaml file (customization purpose)




