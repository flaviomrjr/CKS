FALCO
=====

Reload Falco configuration
```shell
kill -1 $(cat /var/run/falco.pid)
```

File to overwrite Falco rules
`/etc/falco/falco_rules.local.yaml`

Falco config:
`/etc/falco/falco.yaml`