# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout f268d0ddeedc8c485de3ea2f1a33169d6307231f
helm template . --name-template prod-helm-guestbook-east --namespace prod --values ./helm-guestbook/values.yaml --values ./helm-guestbook/values-production-east.yaml --include-crds
```
