# HMCTS PostgreSQL Helm Chart 

This Helm chart deploys PostgreSQL on a Kubernetes cluster using the HMCTS ACR hosted PostgreSQL container image. This is created 
based on the Bitnami PostgreSQL Helm chart locates at ./bitnami/postgresql.

## Chart Templates

`hmcts/postgresql/templates` is a clone of `bitnami/postgresql/templates` without any changes. 

## To install the chart

```bash
az acr login --name hmctsprod.azurecr.io
helm install postgresql hmcts/postgresql --namespace <NAMESPACE> -f hmcts/postgresql/values-simple.yaml
```

