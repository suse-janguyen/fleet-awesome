### Mitigation of Ingress Nightmare

One can disable the admission controller on a vulnerable rke2-ingress-nginx install.

[Description of the Vulerability](https://www.wiz.io/blog/ingress-nginx-kubernetes-vulnerabilities)

#### Mitigation

> _If you have installed ingress-nginx using Helm, reinstall with controller.admissionWebhooks.enabled=false. _

...
