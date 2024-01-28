# Frigate kustomization K8s

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: frigate
  namespace: fleet-default
  labels:
    frigate: enabled
spec:
  branch: main
  clientSecretName: auth-hp48c
  repo: https://github.com/NicoOosterwijk/frigate-k8s.git
  targets:
    - clusterGroup: frigate
```