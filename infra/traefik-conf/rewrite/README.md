### Traefik Rewrite Middleware

Use the rewrite option of Traefik's `MiddleWare` resource to rewrite the [gitjob-webhook](https://fleet.rancher.io/webhook) for Fleet. See the [traefik middlewares documentation](https://doc.traefik.io/traefik/middlewares/http/replacepathregex/) for more information. Requires the GitRepo location like Github or Gitlab to have connectivity and reachability to the Ingress.


