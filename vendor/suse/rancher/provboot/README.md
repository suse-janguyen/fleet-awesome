### Rancher Provisioning Bootstrap

* Note, this should be considered experimental, could go GA in Rancher 2.12.
* Info in the [PR merged here.[(https://github.com/rancher/rancher/pull/46722)

Example sync-bootstrap secret from the QA Testing Considerations -

```
apiVersion: v1
data:
  hello: d29ybGQ=
kind: Secret
metadata:
  annotations:
    rke.cattle.io/object-authorized-for-clusters: prebootstrap-test # cluster name
    provisioning.cattle.io/sync-bootstrap: "true"
    provisioning.cattle.io/sync-target-namespace: kube-system
    provisioning.cattle.io/sync-target-name: hello-synced-yo-world
  name: hello-world
  namespace: fleet-default
type: Opaque
```

Can also use `provisioning.cattle.io/sync` in place of sync-bootstrap so if the requirement is not during provisioning.

_TODO_
- [ ] test with custom clusters, as in the PR
- [ ] differences with Imported clusters? (RKE2 / K3S only).

...

