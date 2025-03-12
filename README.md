## Fleet Awesome

A curated list of minimal reproducible examples, managed by SUSE Rancher Fleet. All assets should be quick and minimal, if customization is necessary, allow flexible config through secrets or downstream cluster `ConfigMap` objects.
Unlike other "awesome-something" lists, the role of Fleet is as a facilitator for gitops operations, the convention, and format of the repo.

## Structure 

 * Infra covers infrastructure-related assets, including CNI configurations, K8s distributions, dual-stack, and ingresses.
 * Location is for cloud-providers, on-premises environments, homelab, KVM, Harvester.
 * Misc is for any topic or asset that does not fit into other categories, or upstream open source projects that might be covered in AppCo.
 * Security for those related topics, secrets, service mesh, mtls.
 * Storage and CSI-related assets, for options in a homelab like minio and NFS.
 * Vendor for vendor-specific assets which may or may not be open source, or have a vendor-component in the asset, manifests, or charts.  The main example is Application Collection.

Initially, the primary topics for the repo are Infra and Vendor/Application Collection.

## TODO: March 2025

- [x] collect and organize initial configurations and charts/manifests/kustomizations
- [x] set up gitjob-webhook, no polling for fleet. URL: `info.kubefred.com`, over cloudflared tunnel
- [x] commit the current/inital working dir tree into gitlab
- [x] 100 assets
 * submit various Bundles for testing, using clusters in homelab (Parslab), `GitRepo`... deploy - test - remove
 * evaluate project mapping, content organization, group naming conventions, subsystem repo structure
 * document TODOs and READMEs for every current asset, flag some for removal or not 
 
## TODO: April 2025
 
 * Secrets management, downstream config separation, asset variable templating
 * Target ClusterGroup Labels categorization, webhook polling tests, cluster variable templating
 * security signatures/checksum and provenance (auto gen via CI?)

## TODO: May 2025

 * Component Testing, Automation (generic CI), QA functionality
 * CI Pipeline, inter-team collaboration, possible presentation, PR/Forks of repo content
 * Future training videos or offline videos, consistent new assets like Elemental, GatewayAPI, ClusterAPI

...
