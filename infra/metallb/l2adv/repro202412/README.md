### MetalLB L2 Adv over OpenVSwitch ovs, 2024-12

Tests are between two different nodes, connected by an OpenVswitch virtual switch. Each node is connect to the switch by their relative `eth1` interface,
keeping the advertisement traffic localized to the vswitch only.
Also includes the L2 `IPAddressPool` for the first node, `L2Advertisement` and two example services for adding an L2-Advertised `LoadBalancer` VIP.
