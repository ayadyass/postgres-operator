---
title: "pgo update pgbouncer"
---
## pgo update pgbouncer

Update a pgBouncer deployment for a PostgreSQL cluster

### Synopsis

Used to update the pgBouncer deployment for a PostgreSQL cluster, such
	as by rotating a password. For example:

	pgo update pgbouncer hacluster --rotate-password
	

```
pgo update pgbouncer [flags]
```

### Options

```
      --cpu string            Set the number of millicores to request for CPU for pgBouncer.
      --cpu-limit string      Set the number of millicores to limit for CPU for pgBouncer.
  -h, --help                  help for pgbouncer
      --memory string         Set the amount of memory to request for pgBouncer.
      --memory-limit string   Set the amount of memory to limit for pgBouncer.
      --no-prompt             No command line confirmation.
  -o, --output string         The output format. Supported types are: "json"
      --replicas int32        Set the total number of pgBouncer instances to deploy. If not set, defaults to 1.
      --rotate-password       Used to rotate the pgBouncer service account password. Can cause interruption of service.
  -s, --selector string       The selector to use for cluster filtering.
      --service-type string   The Service type to use for pgBouncer.
```

### Options inherited from parent commands

```
      --apiserver-url string     The URL for the PostgreSQL Operator apiserver that will process the request from the pgo client. Note that the URL should **not** end in a '/'.
      --debug                    Enable additional output for debugging.
      --disable-tls              Disable TLS authentication to the Postgres Operator.
      --exclude-os-trust         Exclude CA certs from OS default trust store
  -n, --namespace string         The namespace to use for pgo requests.
      --pgo-ca-cert string       The CA Certificate file path for authenticating to the PostgreSQL Operator apiserver.
      --pgo-client-cert string   The Client Certificate file path for authenticating to the PostgreSQL Operator apiserver.
      --pgo-client-key string    The Client Key file path for authenticating to the PostgreSQL Operator apiserver.
```

### SEE ALSO

* [pgo update](/pgo-client/reference/pgo_update/)	 - Update a pgouser, pgorole, or cluster

###### Auto generated by spf13/cobra on 1-Jan-2021
