AUDIT
=====

Request steps:

1. RequestReceived
2. ResponseStarted
3. ResponseComplete
4. Panic

Audit Levels:
- None
- Metadata
- Request
- RequestResponse

Enable audit in kube-apiserver
`--audit-log-path`
`--audit-policy-file`
`--audit-log-maxage=10`
`--audit-log-maxbackup`
`--audit-log-maxsize`