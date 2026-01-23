# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 34ab77484e58cefd7f3c380730b5dc2068fe1920
helm template . --name-template dev-helm-guestbook --values ./helm-guestbook/dev-values.yaml --include-crds
```
