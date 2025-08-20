### L650 Cluster Node
 
A demo single-node RKE2 v1.32.x cluster with Leap Micro 6.1 on mainline kernel-default and a configuration with the following experiments:

 * kube-vip v1.0.0 - L3 Adv 10.16.23.216/29
 * victoria-metrics single-node with grafana
 * traefik `HelmChartConfig` for GatewayAPI 
   * example gateway tcp/8000

#### Notes
 
The following experiments are finished.

 * replacement for n515 failure
 * pihole-svc traefik externalname passthrough
 * unifi-svc traefik externalname passthrough
 * whoami-0a1017d9.nip.io vip (nip.io no longer supports hex-names)
 * tor-controller
 * previous l650 moved to gcp/rky530
 * traefik letsencrypt acme
 * custom-coredns helmchartconfig (see geexology/n515/ )
 * leap-toolbox pod 

---
