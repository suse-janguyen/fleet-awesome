
### Bitwarden Secrets Manager Kubernetes Operator

The sm-operator uses a controller to synchronize Bitwarden secrets into Kubernetes secrets. The operator registers the Custom Resource Definition: BitwardenSecret into the Kubernetes cluster. The cluster will listen for the newly registered BitwardenSecret, and synchronize on a configurable interval.

  * Documentation: https://bitwarden.com/help/secrets-manager-kubernetes-operator/
  * `external-secrets` operator also as a client

...
