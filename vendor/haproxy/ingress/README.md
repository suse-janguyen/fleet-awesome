### Haproxy Ingress 

 * [Documentation](https://github.com/haproxytech/helm-charts/tree/main/kubernetes-ingress)
 * [GatewayAPI / GAPI Docs](https://www.haproxy.com/documentation/kubernetes-ingress/gateway-api/enable-gateway-api/) Note: Current supported version is 0.5.1 -- only supporting TCP Route

_TODO_ 
- [x] fleet bundle, to test - bundle name vendor/haproxytech/haproxy-ingress adds too many chars, >63
- [x] list TCP / GatewayAPI examples (testing... done)
- [x] workaround wit$h extra ttl time of 10d for Job, mitigate issue #2051
- [x] update fleet.yaml bundle for `valuesFrom` in addition to `helm.values` ... keeping in mind spacing issues, now includes values from both places, one is a base and other is downstream customization

...
