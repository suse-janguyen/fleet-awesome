### Volsync

VolSync is a Kubernetes operator that performs asynchronous replication of persistent volumes within, or across, clusters. The replication provided by VolSync is independent of the storage system. This allows replication to and from storage types that don’t normally support remote replication. Additionally, it can replicate across different types (and vendors) of storage.

The chart uses rsync and rclone to perform the operations. Consult [the documentation](https://volsync.readthedocs.io/en/stable/index.html) for more information.

