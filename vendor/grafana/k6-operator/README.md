### Grafana K6 Operator

[Documentation](https://grafana.com/docs/k6/latest/set-up/set-up-distributed-k6/install-k6-operator/)

```
helm install step

helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm install k6-operator grafana/k6-operator

```

_TODO_
- [ ] move test.js files into ConfigMap, refrenced by TestRun CRD.

...
