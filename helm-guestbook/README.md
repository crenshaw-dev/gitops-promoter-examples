# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout bfd64d91079f4c0f98199549acbba40ad1bf804a
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/dev-values.yaml --include-crds
```
