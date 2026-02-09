# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/crenshaw-dev/gitops-promoter-examples
# cd into the cloned directory
git checkout 3a73f30434f79bc671be63d01bdc935db19a9080
helm template . --name-template test --namespace default --include-crds
```
