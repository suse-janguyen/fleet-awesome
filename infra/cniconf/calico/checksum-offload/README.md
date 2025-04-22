### Calico ChecksumOffload Control

From [the docs](https://docs.rke2.io/networking/basic_network_options?CNIplugin=Calico+CNI+Plugin), Linux kernels prior to 5.7 should set this to `true` and `false` for versions 5.7 and higher.

> _Because of a kernel bug in versions previous to 5.7, Calico disables hardware checksum offload. That config caps TCP performance to ~2.5Gbps. If you require higher throughput and have a kernel version greater than 5.7, you can enable the checksum offloading by using the following HelmChartConfig._


