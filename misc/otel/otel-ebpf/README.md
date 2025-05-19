### OpenTelemetry EBPF Chart

The OpenTelemetry eBPF project develops components that collect and analyze telemetry from the operating system, cloud, and container orchestrators. Its initial focus is on collecting network data to enable users to gain insight into their distributed applications.

The kernel collector gathers low level telemetry straight from the Linux kernel using eBPF. It does so with negligible compute and network overheads. The kubernetes collector and cloud collector gather workload metadata.

This telemetry is then sent to the reducer, which enriches and aggregates it. The reducer outputs metrics to the OpenTelemetry collector.


See the [github repo](https://github.com/open-telemetry/opentelemetry-network) for more information.


