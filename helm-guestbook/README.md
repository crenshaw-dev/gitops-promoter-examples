# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 87cf50346ee9ffa7886b63f9559b2b8718b9a4cc
helm template . --name-template staging-helm-guestbook --namespace staging --values ./helm-guestbook/values.yaml --values ./helm-guestbook/staging-values.yaml --include-crds
```
