### Wireugard Tunnel Encryption

* Can configure IPv4, IPv6, or both.
* Configuration `exclude-node` for exempting one node from Wireguard.
* Enabling wireguard tunnel _does not_ disable the `vxlan.calico` interface, as a fallback for the nodes that do not support wireguard. So most nodes will show both vxlan and wireguard interfaces. See https://suse.slack.com/archives/C02BRJYTEHK/p1718182222057329?thread_ts=1718134145.852539&cid=C02BRJYTEHK ... flag for removal later ...
* More details https://docs.tigera.io/calico/latest/network-policy/encrypt-cluster-pod-traffic
