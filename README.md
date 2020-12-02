# Cloud Native PostgreSQL plugin for `kubectl`

Plugin for `kubectl` to manage a Cloud Native PostgreSQL
cluster in Kubernetes. The plugin works also with `oc` in
an OpenShift environment.

For details, please refer to Cloud Native PostgreSQL documentation.

You can install the plugin in your system with:

``` sh
curl -sSfL \
  https://github.com/EnterpriseDB/kubectl-cnp/raw/master/install.sh | \
  sudo sh -s -- -b /usr/local/bin
```

The plugin requires the Cloud Native PostgreSQL operator to be
installed in the Kubernetes/Openshift cluster.
