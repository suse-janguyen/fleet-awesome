### OpenTelemetry Collector Chart

The chart bundle installs OpenTelemetry Operator in a Kubernetes cluster. The OpenTelemetry Operator is an implementation of a Kubernetes Operator. The Operator's Docker image supports only Linux and cannot run on Windows nodes. At this point, it has OpenTelemetry Collector as the only managed component.

* TLS Certificate is Required, it is recommeneded to use `cert-manager` for certificate management.


