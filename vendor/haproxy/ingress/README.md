### Haproxy Ingress 

 * [Documentation](https://github.com/haproxytech/helm-charts/tree/main/kubernetes-ingress)
 * [GatewayAPI / GAPI Docs](https://www.haproxy.com/documentation/kubernetes-ingress/gateway-api/enable-gateway-api/) Note: Current supported version is 0.5.1 -- only supporting TCP Route
 * Fleet [GH Issue #2051](https://github.com/rancher/fleet/issues/2051) for haproxy-ingress `crdjob` pod, fixed in Fleet  > v0.12.0, Rancher 2.12+.

#### Bootstrap Namespace & ConfigMap ####

To work around the issue #2051 under Fleet < v0.12.0, bootstrap the target Cluster's Namespace (`haprpoyxtech`) with a ConfigMap named `haproxy-ingress-values`. An example Kustomization is found under the `bootstrap` directory.

```
---
kind: ConfigMap
apiVersion: v1
metadata:
  name: haproxy-ingress-values
  namespace: haproxytech
data:
  values.yaml: |
    crdjob:
      ttlSecondsAfterFinished: 8640000

###

```

...
