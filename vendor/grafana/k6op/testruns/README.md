### TestRun CRDs for K6-Operator

Makes use of `dependsOn` to ensure the fleet bundle for the K6 Operator is installed first. [Troubleshooting Docs](https://grafana.com/docs/k6/latest/set-up/set-up-distributed-k6/usage/common-options/) for deploying various tests, first two examples are `SmokeTest` and `BreakPoint`.

_TODO_
- [ ] Fleet bundle testing. Changes picked up on gitrepo-push webhook.

...
