### Ngrok Controller

Ngrok tunnel management controller for Kubernetes Ingress.

The ingress-controller will be deprecated soon, should switch to the [ngrok-operator](https://ngrok.com/docs/k8s/installation/install/). 

_TODO_
- [x] depends on above secrets/bootstrap management
- [x] handle credential secrets, `credentials.apiKey` and `credentials.authtoken` from secrets-store/bootstrap secret
- [ ] several ingress examples, including gitops/fleet-gitrepo related webhooks

...
