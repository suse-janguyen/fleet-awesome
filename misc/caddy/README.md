### Caddy Server Helm Chart

Caddy is a webserver written in golang with a lot of advanced features. It is like an NGINX alternative, see [the github repo](https://github.com/caddyserver/caddy) listed here.

The chart itself is bare-bones and configures a PVC called `nfs-static-pvc`, making it ideal for a small experimental lab, http/https backend, local web development, and as a small example of simple helm chart development demo.

Override the default values with a `ConfigMap` or `Secret` downstream.

