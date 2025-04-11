### Secrets Management Workflow

Secrets should never live in git or any repo, see [the fleet docs](https://fleet.rancher.io/gitrepo-add#storing-credentials-in-git), the workflow for secrets management should be separate. There are many best-practice options for this unique workflow.

Every environment's choice of secrets workflow will be context-dependent. In a Lab or Support-Replication environment, simplicity is a key factor, chose the best-suited option for the situation.


* SOPS controller, with AGE or GPG encryption
* OCI private repo with OCI Volumes (Alpha in K8s 1.31+, disabled by default, find the [documentation here](https://kubernetes.io/blog/2024/08/16/kubernetes-1-31-image-volume-source/).
* Secrets Management applications:
  * HashiCorp Vault
  * OpenBao (Hashi Vault Clone)
  * Infisical
  * Local Kustomize manifests
  * BitWarden Secrets Manager (Beta), Note: free tier for lab doesn't isolate by ProjectID, needs multiple machine-accounts to isolate groups of environment secrets.
  * External-Secrets Operator (ESO) as a multi-client to different Providers.
* AppCo wants http-auth in the local/upstream/fleet-conroller `GitRepo` option `helmSecret` while downstream/fleet-agent should have registry-auth.

_TODO_
- [x] ~local Kustomize manifests~
- [x] ~test moving between local/agents, different namespaces, `BundleNamespaceMapping` [documentation](https://fleet.rancher.io/multi-user#allow-access-to-clusters)~
- [x] ~secrets workflow as a series of bootstrap objects, like `GitRepo` that can also populate a namespace with the secret, any configmaps (for `valuesFrom`), gitrepo examples for any fleet-controller.~

...
