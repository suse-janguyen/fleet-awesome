### K8S Dual Stack

 * [Documentaion](https://kubernetes.io/docs/concepts/services-networking/dual-stack/)
 * Sample `config.yaml` for RKE2 & K3S
 * IPv6 Requires a working default-gateway, even if the gw is just to a `dummy0` interface
 * Node-CIDRs fit inside Cluster-CIDRs
 * Services configuration for `.spec.ipFamilies` for IPv4, IPv6, or Both
 * Services `.spec.ipFamilyPolicy` options are `PreferDualStack`/`RequireDualStack` (both equivalent) or `SingleStack`

_TODO_
- [ ] examples for dual or single-stack services
- [ ] combine with multus for separation of ip families

...
