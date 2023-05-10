Syscalls
========

Strace inspecs the syscalls makes from commands
```shell
strace touch /tmp/error.log
```

Get the PID from service
```shell
pidof etcd
```

Check the syscalls from a pid
```shell
strace -p 3596
```

Check multi syscalls
```shell
strace -c touch /tmp/error.log
```