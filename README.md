### argocd

## Install ArgoCD:  <br />
  ```kubectl create namespace argocd``` <br />
  ```kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml```


## Get Password: <br />
  ```kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo```

## Setup Application & Project: <br />
  https://argo-cd.readthedocs.io/en/stable/operator-manual/declarative-setup/

