### Sublevel Cluster Nodes
 
_Description:_
 * Rancher downstream import to main instance rancher.kubefred, physical machines
 * cert-manager, gcore-webhook, cf-dns01 and gc-dns01 ClusterIssuers 
 * fleet-controller 0.11.5 standalone for r127 fleet-agent
 * nfs-subdir-external-provisioner nfs-client 
 * sm-operator beta testing, postgresql 17.0 manifest testing
 * cloudflared tunnel for info.kubefred, currently gitjob-webook dedicated host
 * kube-vip L3 Adv BGP VIP 10.16.23.224/29
 * vip LB services for postgres, traefik-dashboard, traefik-vip

_TODO_
- [x] Add Primary `GitRepo` to fleet-controller
- [x] Alter GitRepo name so Bundles aren't named like ~sublevel-location-parselab-sublevel~ now uses `fawesome` placeholder
- [ ] Optional Additional GitRepo resources
- [ ] Add inital `CusterGroups` for testing
- [ ] fleet-controller options 
   * `.spec.correctDrift.enabled` = true for Resource Handling: Enable Self-Healing in UI 
   * `.spec.keepResources' = true for Resource Handling: Always Keep Resources in UI

...
