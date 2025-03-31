### Grafana K6 Operator

The k6-operator uses two CRDs, `TestRun` and  `PrivateLoadZones`, with the latter integrated with Grafana Cloud K6, this repo covers an example of the TestRun custom resource.

[Documentation](https://grafana.com/docs/k6/latest/set-up/set-up-distributed-k6/install-k6-operator/)

```
helm install step

helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm install k6-operator grafana/k6-operator
...

kubectl create configmap smoke-test --from-file=smoke.js  --dry-run=client -o yaml 
kubectl create configmap breakpoint --from-file=breakpoint.js --dry-run=client -o yaml

```

_TODO_
- [x] move test.js files into ConfigMap, refrenced by TestRun CRD.
- [x] fleet bundle for operator and then TestRun example (`dependsOn`)

...
