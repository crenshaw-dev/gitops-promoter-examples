# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 416d21b2a28be83d13c648d966c5d2038ad9d460
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/values.yaml --include-crds
```
