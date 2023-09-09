1. ### Lens K8s app [Add a cluster](https://docs.k8slens.dev/getting-started/add-cluster/):
    1. To add a cluster manually:
       1. ```minikube start```
       2. ```minikube ip```
    2. To see your current cluster configuration:
       1. ```kubectl config view --minify --raw```



       
    3. Install the cert-manager Helm chart:
       1. ```
          1. helm install \
          2. cert-manager jetstack/cert-manager \
          3. --namespace cert-manager \
          4. --create-namespace \
          5. --version v1.8.0 \
          6. --set installCRDs=true
          ```
    4. Update ingress-service.yaml
    5. Create certificate.yaml
    6. Create issuer.yaml
