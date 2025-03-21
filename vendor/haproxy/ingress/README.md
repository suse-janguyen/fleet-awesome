### Haproxy Ingress 

 * [Documentation](https://github.com/haproxytech/helm-charts/tree/main/kubernetes-ingress)
 * [GatewayAPI / GAPI Docs](https://github.com/haproxytech/helm-charts/tree/main/kubernetes-ingress#installing-gateway-api-support) Note: Current supported version is 0.5.1 -- only supporting TCP Route

_TODO_ 
- [x] fleet bundle, to test - bundle name vendor/haproxytech/haproxy-ingress adds too many chars, >63
- [x] list TCP / GatewayAPI examples (testing... done)
- [ ] Optional, a bundle-diff patch [see docs](https://fleet.rancher.io/bundle-diffs), to ignore the haproxy-ingress-crjob ... if one deletes the Job, the Bundle goes unready, even if it's in `Status: Succeeded` (Completed).

...
