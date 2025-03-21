### Fleet-Controller

The `sublevel` cluster is a downstream of Rancher, but acts as a controller for "fleet-of-fleets" where a newer, experimental version of Fleet lives. This has implications for hosted services.

* webhook for polling, `disablePolling: true`
* foundation established with namespaces, secrets, and configmaps for variable mapping, `keepResources: true` 
  * _(do not remove those resources if gitrepo targets are removed...)_

_TODO_
- [x] `overrideTargets` for fleet.yaml bundles, override the targets from the GitRepo, tested w/ pihole chart & ClusterGroups
- [x] `targetCustomizations` specifically for helm values, ex: modify values for specific environments
- [ ] bundle namespace mapping, [see the documentation](https://fleet.rancher.io/namespaces#cross-namespace-deployments)

...
