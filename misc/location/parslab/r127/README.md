### R127 Cluster Node
 
Current status:

 * fleet-agent 0.11.5 to sublevel controller, downstream target cluster
 * in `clusters` namespace, may need to rename
 * L2 Adv Metallb-VIP 10.16.24.0/26
 * helmchartconfigs for canal-wireguard, ingress-nginx, multus-whereabouts
 * minio storage0 manifest with nfs3 backend
 * optional svc-vips for minio & pihole
 * Dec15-2023 repro whereabouts ranges

_TODO_
- [ ] preconfigure configmaps in namespaces, ie for haproxytech

...
