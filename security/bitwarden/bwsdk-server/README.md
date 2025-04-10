### Bitwarden SDK Server

The main purpose of this API is to accommodate the needs for External Secrets Operator to talk to Bitwarden Secrets Manager.

Notes: 

  * Requires Cert-Manager and the bootstrap Cluster Issuer & Certificate, Kustomization under `/security/bitwarden/sdkboot`
  * for the upstream `external-secrets` chart, this is included, enable with `bitwarden-sdk-server.enabled=true` helm value.  
  * for the Application Collection (SUSE/Rancher), it is not included so the above value does nothing, instead one can opt to add this chart to their fleet GitRepo paths, as part of a larger recipe/stack/snippet.
  * successful install provides an https/443 Service on port 9998

