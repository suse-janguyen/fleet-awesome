### External Secrets Operator (ESO)

Synchronize secrets from many Providers, similar to Rancher's provisioning-sync or bootstrap-sync controllers.
This package is built by Application Collection from upstream sources.

See the [AppCo Docs](https://apps.rancher.io/applications/external-secrets-operator) for more information.

Notes: 

* The upstream developers only [test against](https://external-secrets.io/latest/introduction/stability-support/) the latest version of Kubernetes.
* This chart does not include `bitwarden-sdk-server`, so the helm option `bitwarden-sdk-server.enabled=true` does not install the sdk. It does work if installed individually.

_TODO_
- [x] pre-configure secret with appco auth
- [x] pre-configure configmap with gloabal.`imagePullSecrets` ... (accesstoken, serviceacct gives 403)
- [x] tests with K8S 1.30, 1.31 with ESO 0.14.x 
- [x] cert issuer for `bitwarden-sdk-server` to satisfy bitwarden-tls-certs` requirement 
- [ ] separate chart, bundle, tls-secrets bootstrap for `bitwarden-sdk-server`
- [ ] use `PushSecret` to move between clusters and providers, [docs for the CRD](https://external-secrets.io/latest/guides/pushsecrets/)

...
