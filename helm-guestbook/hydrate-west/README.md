# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 294e95094ecb540364fb5b90585b8bb09abd90d3
helm template . --name-template prod-helm-guestbook-west --namespace prod --values ./helm-guestbook/values.yaml --values ./helm-guestbook/values-production-west.yaml --include-crds
```
