# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 1b87995ed8f69ba6b4430a648dc13f818b669594
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/values.yaml --include-crds
```
