Service Accounts
================

## Manage Service Accounts 

```shell
kubectl create sa test

kubectl get sa

kubectl describe sa test

kubectl describe secret test-sa-token-kbbdm
# Toda SA possui uma secret com seu token
```

Secrets path

```shell
kubectl exec -ti my-pod -- ls /var/run/secrets/kubernetes.io/serviceaccount

kubectl exec -ti my-pod -- cat /var/run/secrets/kubernetes.io/serviceaccount/token
```

Disable auto service account mount in pods:

Set: `automountServiceAccountToken: false`

## Changes in versions 1.22 and 1.24

Bound Service Account Tokens

Redunction of Secret-based Service Account Tokens

In case you want a token you must creat a secret and then a token:

```shell
kubectl create serviceaccount test

kubectl create token test
```

To create secrets in the old version add this annotation:

```yaml
annotations:
    kubernetes.io/service-account.name: test (Service account name)