# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 4dd37efc6d9021b6f309ee55dd6da41259d3b911
helm template . --name-template staging-helm-guestbook --namespace staging --values ./helm-guestbook/values.yaml --values ./helm-guestbook/staging-values.yaml --include-crds
```
