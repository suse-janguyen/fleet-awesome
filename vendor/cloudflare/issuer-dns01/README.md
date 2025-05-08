### CloudFlare DNS01 Cert-Manager Issuer

This snippet places the `Issuer` into the `cattle-system` namespace, requires an existing api-key secret named `cloudflarei-api-token-secret` in the same namespace.
See the [cert-manager cloudflare](https://cert-manager.io/docs/configuration/acme/dns01/cloudflare/) dns01 documentation for more information.

