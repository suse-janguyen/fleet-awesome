### KubeVirt Operator

Currently version 1.5.1, for Kubernetes 1.30, 1.31, and 1.32. See the [user guide](https://kubevirt.io/user-guide/) for more information.

_TODO_

User guide mentions operator first, then CR definitions afterwards.
Bundle complains Namespace is not owned by Helm, see error below.

```
NotReady(1) [Cluster fleet-default/rocky-530: not installed: Unable to continue with install: Namespace "kubevirt" in namespace "" exists and cannot be imported into the current release: invalid ownership metadata; label validation error: missing key "app.kubernetes.io/managed-by": must be set to "Helm"; annotation validation error: missing key "meta.helm.sh/release-name": must be set to "kubevirt"; annotation validation error: missing key "meta.helm.sh/release-namespace": must be set to "kubevirt"]
```

* Bootstrap Namespace as part of kustomization

