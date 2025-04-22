## Infrastructure Assets

The infrastructure group falls into two main categories of classification. Every asset has a call-out in the README in which category they fall into, this could be changed, altered, or reorganized in the future.

* Bootstrap Infra. Cloud Providers, Custom and Provisioned Rancher Clusters. Clusters provsioned by a third-party like AWS-ACK, Flux,  terraform or tofu, and Imported Clusters. Sometimes these are not directly deployable via GitOps with Fleet.
* Fleet GitOps Deployments. These include enhancements or configurations after-the-fact. Metallb, Multus, CoreDNS, Traefik, Ingress-Nginx, CNI-specific configurations, and other `HelmChartConfig` resources consumable by RKE2 & K3S.

...
