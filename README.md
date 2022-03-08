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

## Windows install

To install the plugin on Windows go to the [releases
page](https://github.com/EnterpriseDB/kubectl-cnp/releases) and get the most
recent release for your Windows architecture.

For example, if you are using an `x86_64` build of Windows, you would download
the file named `kubectl-cnp_<version>_windows_x86_64.tar.gz`.

The release includes a checksum file, named
`kubectl-cnp-<version>-checksums.txt`, that can be used to validate the
integrity of the Kubectl binary.

To validate the file you can compare the output of the following command
against the relative line in the checksums file:

```
CertUtil -hashfile <tar-file> SHA256

type <tar-file>.sha256
```

Now you can extract the contents of the TAR archive using the following
command:

```
tar xvzf <tar-file>
```

You can copy the `kubectl-cnp.exe` file in any directory pointed by your `PATH`
environment variable, or prepend or append the Kubectl Cnp binary folder to
your `PATH` environment variable.

The directory where `kubectl.exe` is is usually a good choice for copying the
`kubectl-cnp.exe` file to.

