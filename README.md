# Cloud Native PostgreSQL plugin for `kubectl`

Plugin for `kubectl` to manage a Cloud Native PostgreSQL
cluster in Kubernetes. The plugin works also with `oc` in
an OpenShift environment.

For details, please refer to Cloud Native PostgreSQL documentation.

## Mac OS and Linux install
You can install the plugin in your system with:

``` sh
curl -sSfL \
  https://github.com/EnterpriseDB/kubectl-cnp/raw/main/install.sh | \
  sudo sh -s -- -b /usr/local/bin
```

The plugin requires the Cloud Native PostgreSQL operator to be
installed in the Kubernetes/Openshift cluster.

## Windows Install

The best way to install the plugin on Windows is go to the [releases page](https://github.com/EnterpriseDB/kubectl-cnp/releases) and get the most recent release for your Windows architecture. For example, if you are using x86_64 Windows you would [download the x86_64 architecture version](https://github.com/EnterpriseDB/kubectl-cnp/releases/download/v1.13.0/kubectl-cnp_1.13.0_windows_x86_64.tar.gz).

OPTIONAL: you can then check the hash of the **tar file** that you downloaded by running:
```
CertUtil -hashfile kubectl-cnp_1.13.0_windows_x86_64.tar.gz SHA256
```
where "kubectl-cnp_1.13.0_windows_x86_64.tar.gz" would be subsituted with the name of the **tar file** that you downloaded. 
You will compare the hash from the above CertUtil command with the hash next to the version of kubectl-cnp that you downloaded in the [checksums.txt](https://github.com/EnterpriseDB/kubectl-cnp/releases/download/v1.13.0/kubectl-cnp-1.13.0-checksums.txt) file.

Now you can add the ```kubectl-cnp.exe``` to the same directory that contains your ```kubectl.exe``` to use the plugin.

