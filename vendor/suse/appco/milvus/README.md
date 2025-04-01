### Milvus Chart

Milvus is a high-performance vector database built for scale. It is used by AI applications to organize and search through large amount of unstructured data, such as text, images, and multi-modal information.

```
helm pull oci://dp.apps.rancher.io/charts/milvus --version 4.2.2
```
Requires the following dependency charts:
* Apache Kafka
* Etcd
* Minio

See [Application Collection Documentation](https://apps.rancher.io/applications/milvus) for this chart.

_TODO_
- [ ] test install/uninstall, with minimal values if possible

...
