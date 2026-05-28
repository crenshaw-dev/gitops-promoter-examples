# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout c2355aa5b2a794256a24a3b26cb3e1a17fb5c068
helm template . --name-template prod-helm-guestbook-east --namespace prod --values ./helm-guestbook/values.yaml --values ./helm-guestbook/values-production-east.yaml --include-crds
```
