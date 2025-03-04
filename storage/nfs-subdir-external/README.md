### NFS Subdir Provisioner

* add values for server address & path ...

$ helm install nfs-subdir-external-provisioner nfs-subdir-external-provisioner/nfs-subdir-external-provisioner \
    --set nfs.server=x.x.x.x \
    --set nfs.path=/exported/path

... could be downstream configmap in fleet.yaml bundle

