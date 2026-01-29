# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 294e95094ecb540364fb5b90585b8bb09abd90d3
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/dev-values.yaml --include-crds
```
