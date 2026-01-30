# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 89a88f7e4ade23f336a724f7776188e7ebdd71b5
helm template . --name-template prod-helm-guestbook-west --namespace prod --values ./helm-guestbook/values.yaml --values ./helm-guestbook/values-production-west.yaml --include-crds
```
