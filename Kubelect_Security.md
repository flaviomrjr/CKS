Kubelet Security
=================

Kubelet are not deployed by KubeAdm you must install in each node.

Kubelet port:
- 10250: Full Access
- 10255: Ready Only

Some flags:
--anonymous-auth=false

--client-ca-file

--authorization-mode=WebHook

--read-only-port=0
