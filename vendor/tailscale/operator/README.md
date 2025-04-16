### Tailscale Operator

Tailscale Kubernetes Operator.

[Documentation](https://tailscale.com/kb/1236/kubernetes-operator) as a KB article.
[Github Repo](https://github.com/tailscale/tailscale/blob/main/cmd/k8s-operator/deploy/) for the helm chart.

* Chart will mount `oauth.clientId` and `oauth.clientSecret` values inside `oauthSecretVolume` by default.
* Value `ingressClass.enabled`: true as default

