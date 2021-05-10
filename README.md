## Prereq

[kustomize-v4.1.2](https://github.com/kubernetes-sigs/kustomize/releases/tag/kustomize%2Fv4.1.2)

## Config

```
kustomize cfg set . IMAGE_NAME <image-name> 
kustomize cfg set . TAG_NAME <tag-name>
kustomize cfg set . NAMESPACE_NAME <namespace-name> 
kustomize cfg list-setters . --include-subst
```

## Deploy

kustomize build | kubectl apply -f -

## Undeploy

kustomize build | kubectl delete -f -
