---
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  annotations:
    field.cattle.io/description: github generic-example
  name: generic-example
  namespace: fleet-default
spec:
  branch: main
  paths:
  - /storage/local-path-prov
  pollingInterval: 300s
  repo: https://github.com/your-username/yourfork-fleet-awesome
  targets:
  - name: localpath
    clusterGroupSelector:
      matchLabels:
        rancher-localpath-prov: enabled