# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout f2fec971ec2eef4af29461e5936fc1df5c6ea48e
helm template . --name-template prod-helm-guestbook-east --namespace prod --values ./helm-guestbook/values-production-east.yaml --include-crds
```
