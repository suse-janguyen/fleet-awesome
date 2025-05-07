### SUSE Rancher Application Collection

A curated list of some AppCo helm charts. Personal access-token or organization service-account is required. 

_Note on authentication_
  * the local cluster fleet-controller's `GitRepo` requires http-auth for a `helmSecret` option.
  * Downstream authentication requires type registry-auth secrets
  * Bootstrap the targetting destination namespace with the Secrets (registry-auth) and ConfigMap for `valuesFrom` in the fleet.yaml Bundle.


#### Example GitRepo ####

 * See [the Fleet docs](https://fleet.rancher.io/gitrepo-add#using-http-auth) for more info about GitRepo authentication.
 * `appco-accesstoken-http` is http-auth with `.data.username` and `.data.password`
 * the target cluster is local, target namespace for the chart is external-secrets, so bootstrap the namespace with a secret called `appco-accesstoken-registryauth` 
 * the fleet-controller pulls the appco chart with the http-auth secret, the fleet-agent pulls the appco chart with the registry-auth imagePullSecret, see [the AppCo docs](https://docs.apps.rancher.io/howto-guides/integrate-with-rancher-manager/) for more info about Rancher and the registryauth imagePullSecrets integration.

```
...

spec:
  branch: main
  helmRepoURLRegex: (oci|https)://dp.apps.rancher.io/*
  helmSecretName: appco-accesstoken-http
  paths:
    - /vendor/suse/appco/external-secrets
  repo: https://github.com:flrichar/fleet-awesome
  targets:
    - clusterName: local

...

```

