# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 8a2e3b1a2e903e89d6a6735389ba860e783304f4
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/dev-values.yaml --include-crds
```
