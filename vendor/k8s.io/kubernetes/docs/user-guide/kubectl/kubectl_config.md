<!-- BEGIN MUNGE: UNVERSIONED_WARNING -->


<!-- END MUNGE: UNVERSIONED_WARNING -->

## kubectl config

config modifies kubeconfig files

### Synopsis


config modifies kubeconfig files using subcommands like "kubectl config set current-context my-context"

The loading order follows these rules:
1. If the --kubeconfig flag is set, then only that file is loaded.  The flag may only be set once and no merging takes place.
2. If $KUBECONFIG environment variable is set, then it is used a list of paths (normal path delimitting rules for your system).  These paths are merged together.  When a value is modified, it is modified in the file that defines the stanza.  When a value is created, it is created in the first file that exists.  If no files in the chain exist, then it creates the last file in the list.
3. Otherwise, ${HOME}/.kube/config is used and no merging takes place.


```
kubectl config SUBCOMMAND
```

### Options

```
      --kubeconfig="": use a particular kubeconfig file
```

### Options inherited from parent commands

```
      --alsologtostderr[=false]: log to standard error as well as files
      --certificate-authority="": Path to a cert. file for the certificate authority.
      --client-certificate="": Path to a client certificate file for TLS.
      --client-key="": Path to a client key file for TLS.
      --cluster="": The name of the kubeconfig cluster to use
      --context="": The name of the kubeconfig context to use
      --insecure-skip-tls-verify[=false]: If true, the server's certificate will not be checked for validity. This will make your HTTPS connections insecure.
      --log-backtrace-at=:0: when logging hits line file:N, emit a stack trace
      --log-dir="": If non-empty, write log files in this directory
      --log-flush-frequency=5s: Maximum number of seconds between log flushes
      --logtostderr[=true]: log to standard error instead of files
      --match-server-version[=false]: Require server version to match client version
      --namespace="": If present, the namespace scope for this CLI request.
      --password="": Password for basic authentication to the API server.
  -s, --server="": The address and port of the Kubernetes API server
      --stderrthreshold=2: logs at or above this threshold go to stderr
      --token="": Bearer token for authentication to the API server.
      --user="": The name of the kubeconfig user to use
      --username="": Username for basic authentication to the API server.
      --v=0: log level for V logs
      --vmodule=: comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO

* [kubectl](kubectl.md)	 - kubectl controls the Kubernetes cluster manager
* [kubectl config current-context](kubectl_config_current-context.md)	 - Displays the current-context
* [kubectl config set](kubectl_config_set.md)	 - Sets an individual value in a kubeconfig file
* [kubectl config set-cluster](kubectl_config_set-cluster.md)	 - Sets a cluster entry in kubeconfig
* [kubectl config set-context](kubectl_config_set-context.md)	 - Sets a context entry in kubeconfig
* [kubectl config set-credentials](kubectl_config_set-credentials.md)	 - Sets a user entry in kubeconfig
* [kubectl config unset](kubectl_config_unset.md)	 - Unsets an individual value in a kubeconfig file
* [kubectl config use-context](kubectl_config_use-context.md)	 - Sets the current-context in a kubeconfig file
* [kubectl config view](kubectl_config_view.md)	 - Displays merged kubeconfig settings or a specified kubeconfig file.

###### Auto generated by spf13/cobra on 2-Mar-2016



<!-- BEGIN MUNGE: IS_VERSIONED -->
<!-- TAG IS_VERSIONED -->
<!-- END MUNGE: IS_VERSIONED -->


<!-- BEGIN MUNGE: GENERATED_ANALYTICS -->
[![Analytics](https://kubernetes-site.appspot.com/UA-36037335-10/GitHub/docs/user-guide/kubectl/kubectl_config.md?pixel)]()
<!-- END MUNGE: GENERATED_ANALYTICS -->