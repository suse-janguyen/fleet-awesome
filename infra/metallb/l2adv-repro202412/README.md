### MetalLB L2 Adv over OpenVSwitch ovs, 2024-12

Tests worked between r127 & zalg113
changed ippool from 10.100.100.72/29 to 10.16.24.0/26

Idea is new ipam is in /23 increments,
- 10.16.22.0/23 (ovs + bgp-vip00)
- 10.16.24.0/25 (l2-vip01)

Below example configs no longer necessary
Old commeents from IPAddressPool.yaml manifest:
  ###- 10.100.100.72/29
  ###- fda0:b740:e5e0:1000::/64

