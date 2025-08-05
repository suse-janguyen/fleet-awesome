### Istio Migration Report

As of Istio 1.24, the upstream project has deprecated the `IstioOperator` in favor of Helm. Why is this important? The `rancher-istio` chart is a wrapper for the `istioctl` command and installs like the old, now deprecated istio operator.

Users are urged to use the Helm chart for Istio 1.25+, and the `rancher-istio` chart is being deprecated as of Rancher 2.12 and unsupported in Rancher 2.13.  The SUSE Rancher Application Collection is also a Helm chart, and follows the same convention as the upstream project.

Current customers -- or Support Engineers -- may have existing `rancher-istio` installs, with varying configuration. This Fleet Awesome bundle Job performs the following operations: 

* install a temporary Job with an `istioctl` 1.25 init-container
* find the `istio-installer-base.yaml` that was used to install Istio
* output a report on what steps could be taken for each Istio component and configuration

This report will act as a helper for migrating from an old operator-based install to a newer helm-based install. The Fleet Bundle is an alternative to running the commands by hand in a terminal. The report is read with a command `kubectl logs -n istio-system job/istio-report`.

For more information see the [blog post](https://istio.io/latest/blog/2024/in-cluster-operator-deprecation-announcement/#migrating-to-helm) mentioned in the upstream Istio documentaiton.

_TODO_
- [ ] make the Job more friendly and save the other files, yaml, and shell-scripts

---
