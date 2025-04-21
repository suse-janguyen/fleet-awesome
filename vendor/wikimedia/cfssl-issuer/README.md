### Wikimedia CFSSL Issuer

A cert-manager external issuer to request certificates signed by CFSSL API. Useful for running a private CA inside your own lab or organization.

  * Docs: https://gerrit.wikimedia.org/r/plugins/gitiles/operations/software/cfssl-issuer
  * Adds new CRDs like `issuers.cfssl-issuer.wikimedia.org` and `clusterissuers.cfssl-issuer.wikimedia.org` besides the CRDs for the standard cert-manager chart.
  * Chart `dependsOn` cfssl-issuer-crds installed previously.
  * An [example integration](https://linuxera.org/integrating-cert-manager-with-cfssl-multirootca/) refrencing the cfssl-issuer.


