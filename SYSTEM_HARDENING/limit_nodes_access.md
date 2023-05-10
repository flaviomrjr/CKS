Nodes Hardening
===============

Get running services
```shell
systemctl list-units --type service
```

Manage modules:
```shell
# add
modprobe pcspkr

# list
lsmod

# blacklist
blacklist sctp
```

Add user:

useradd -d /opt/sam -s /bin/bash -G admin -u 2328 sam

Remove login:
usermod -s /usr/sbin/nologin himanshi

Add user to group:
usermod rob -G admin

Copy key:
ssh-copy-id -i ~/.ssh/id_rsa.pub jim@node01

Listar pacote:
apt list --instaled

List service:
systemctl list-units --type service

Add to black list kernel module
vim /etc/modprobe.d/blacklist.conf

