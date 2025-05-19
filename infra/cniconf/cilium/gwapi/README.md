### Cilium Gateway API

This fleet bundle configures the Cilium CNI for various options to support Gateway API, including:
  * KubeProxy Replacement 
  * BGP Control Plane
  * LB-IPAM

The kustomization installs the CRDs for GatewayAPI 1.2.0 first including the experimental TLSRoute before configuring the Helm chart with a `HelmChartConfig` resource. See the [upstream docs](https://docs.cilium.io/en/stable/network/servicemesh/gateway-api/gateway-api/) for more information.


