### Cloudflared Client (Formerly Argo Tunnel) 

 Allows global Cloudflare CDN to act as LB for Kubernetes services. Only two objects, a Deployment and ConfigMap, the ingress config is done via the ConfigMap. Not many options for regex or L7 path filtering/redirects. Free tier is limited to a low amount of bandwidth, good for lab use and testing.

 * [Documentation](https://developers.cloudflare.com/cloudflare-one/tutorials/many-cfd-one-tunnel/#upload-the-tunnel-credentials-file-to-kubernetes)
 * Depends on bootstrapped secret `tunnel-credentials`

...
 
