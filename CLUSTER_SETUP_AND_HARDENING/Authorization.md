Authorization
=============

Set flag: `authorization-mode=Node, RBAC, WebHook`

This flag sets que authorization flow!

Default: AlwaysAllow

How to check access:
```shell
kubectl auth can-i create deploy

kubectl auth can-i create deploy --as dev-user
```