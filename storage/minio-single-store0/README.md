### Minio Single Pod NFS 

 This is a small, single-pod deployment of Minio, with an NFS backend as a proof-of-concept. The NFS mount is very simple, not a full-fledged CSI plugin, making this ideal for introducing an S3 compatible storage option to existing NFS backends. Volume is RWO so there is no redudancy, recommended for lab-use only. 

 * uses CFSSL Issuer, TODO: introduce LE Issuer for nginx ingress controller
 * TODO: Deployment `.spec.template.spec.containers.image` as a variable to control minio version

