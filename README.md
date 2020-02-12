# Kubernetes RBAC Groups
### Kubernetes Version: v1.17 (2020-02-12)
Full list of all available default api groups including their resources.

This is a little helper to build RBAC roles for your cluster. Below the group folders are the resources with the following format:

**Example: apps_v1/deployments.yaml**
```
apiGroups:
- apps/v1
resources:
- deployments
verbs:
- create
- delete
- deletecollection
- get
- list
- patch
- update
- watch
```

You will find a complete list of all available verbs for a resource, which can be copied as a rule into an RBAC role.

## Directory Structure

```
.
|-- admissionregistration.k8s.io_v1beta1
|   |-- mutatingwebhookconfigurations.yaml
|   `-- validatingwebhookconfigurations.yaml
|-- apiextensions.k8s.io_v1beta1
|   |-- customresourcedefinitions.yaml
|   `-- customresourcedefinitions_status.yaml
|-- apiregistration.k8s.io_v1
|   |-- apiservices.yaml
|   `-- apiservices_status.yaml
|-- apps_v1
|   |-- controllerrevisions.yaml
|   |-- daemonsets.yaml
|   |-- daemonsets_status.yaml
|   |-- deployments.yaml
|   |-- deployments_scale.yaml
|   |-- deployments_status.yaml
|   |-- replicasets.yaml
|   |-- replicasets_scale.yaml
|   |-- replicasets_status.yaml
|   |-- statefulsets.yaml
|   |-- statefulsets_scale.yaml
|   `-- statefulsets_status.yaml
|-- authentication.k8s.io_v1
|   `-- tokenreviews.yaml
|-- authorization.k8s.io_v1
|   |-- localsubjectaccessreviews.yaml
|   |-- selfsubjectaccessreviews.yaml
|   |-- selfsubjectrulesreviews.yaml
|   `-- subjectaccessreviews.yaml
|-- autoscaling_v1
|   |-- horizontalpodautoscalers.yaml
|   `-- horizontalpodautoscalers_status.yaml
|-- batch_v1
|   |-- jobs.yaml
|   `-- jobs_status.yaml
|-- certificates.k8s.io_v1beta1
|   |-- certificatesigningrequests.yaml
|   |-- certificatesigningrequests_approval.yaml
|   `-- certificatesigningrequests_status.yaml
|-- coordination.k8s.io_v1
|   `-- leases.yaml
|-- events.k8s.io_v1beta1
|   `-- events.yaml
|-- extensions_v1beta1
|   |-- daemonsets.yaml
|   |-- daemonsets_status.yaml
|   |-- deployments.yaml
|   |-- deployments_rollback.yaml
|   |-- deployments_scale.yaml
|   |-- deployments_status.yaml
|   |-- ingresses.yaml
|   |-- ingresses_status.yaml
|   |-- networkpolicies.yaml
|   |-- podsecuritypolicies.yaml
|   |-- replicasets.yaml
|   |-- replicasets_scale.yaml
|   |-- replicasets_status.yaml
|   |-- replicationcontrollers.yaml
|   `-- replicationcontrollers_scale.yaml
|-- metrics.k8s.io_v1beta1
|   |-- nodes.yaml
|   `-- pods.yaml
|-- networking.k8s.io_v1
|   `-- networkpolicies.yaml
|-- node.k8s.io_v1beta1
|   `-- runtimeclasses.yaml
|-- policy_v1beta1
|   |-- poddisruptionbudgets.yaml
|   |-- poddisruptionbudgets_status.yaml
|   `-- podsecuritypolicies.yaml
|-- rbac.authorization.k8s.io_v1
|   |-- clusterrolebindings.yaml
|   |-- clusterroles.yaml
|   |-- rolebindings.yaml
|   `-- roles.yaml
|-- scheduling.k8s.io_v1
|   `-- priorityclasses.yaml
`-- storage.k8s.io_v1
    |-- storageclasses.yaml
    |-- volumeattachments.yaml
    `-- volumeattachments_status.yaml
```



## Contributing

-   **Fork** the project
-   **Patch** some code
-   **Push** your changes
-   Create a **Pull Request**

## Authors

-   Chris Bargmann (@[cbrgm](https://github.com/cbrgm))

## License

```
This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org>
```
