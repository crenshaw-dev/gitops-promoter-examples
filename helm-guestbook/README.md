# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 12ce1e97abdba94b2f04c318e9e5c4615d42186a
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/values.yaml --include-crds
```
