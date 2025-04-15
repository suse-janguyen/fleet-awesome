### Local Path Provisioner

Currently for testing kustomize manifests. Working... Clusters are targeted via GitRepo, clusterGroupSelector in the ClusterGroup labels that match the application, move Clusters into and out of ClusterGroups, add/remove labels to enable different apps in each ClusterGroup.

_TODO_
- [x] apply to agent clusers via label on controller object
- [ ] RKE2 uses kube-system namespace, default ns for chart/manifest is local-path-provisioner

...
