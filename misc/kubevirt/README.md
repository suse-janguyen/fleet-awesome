### KubeVirt Operator

Currently version 1.5.1, for Kubernetes 1.30, 1.31, and 1.32. See the [user guide](https://kubevirt.io/user-guide/) for more information.

* Requires the CRDs Bundle installed first with a ready status
* Operator manifest and kustomization under `operator` directory, with `dependsOn` set to the CRD Bundle


