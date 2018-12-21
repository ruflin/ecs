## Kubernetes use case

You can monitor containers running in a Kubernetes cluster by adding Kubernetes-specific information under `kubernetes.`


### <a name="kubernetes"></a> Kubernetes fields


| Field  | Description  | Level  | Type  | Example  |
|---|---|---|---|---|
| <a name="id"></a>*id* | ** | (use case) |  | `fdbef803fa2b` |
| <a name="name"></a>*name* | ** | (use case) |  |  |
| <a name="hostname"></a>*hostname* | ** | (use case) |  | `kube-high-cpu-42` |
| <a name="pod.name"></a>*pod.name* | *Kubernetes pod name<br/>* | (use case) | keyword | `foo-webserver` |
| <a name="namespace"></a>*namespace* | *Kubernetes namespace<br/>* | (use case) | keyword | `foo-team` |
| <a name="labels"></a>*labels* | *Kubernetes labels map<br/>* | (use case) | object |  |
| <a name="annotations"></a>*annotations* | *Kubernetes annotations map<br/>* | (use case) | object |  |
| [container.name](../README.md#container.name)  | Kubernetes container name. This name is unique within the pod only. It is different from the `container.name` field.<br/> | extended | keyword |  |



