### Cilium BGP ControlPlane v2

These manifests configure Cilium for RKE2 with a `HelmChartConfig`, configure BGP with `CiliumBGPClusterConfig` for the cluster and `CiliumBGPPeerConfig` for a sample Peer selecting only the included `CiliumBGPAdvertisement` with a certain label.  An example Service, `ServiceExcalidrawVIP` is included for testing.

See the [Cilium BGP Control Plane v2](https://docs.cilium.io/en/latest/network/bgp-control-plane/bgp-control-plane-v2/) documentation for more detail.


