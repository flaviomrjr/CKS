UFW
===

```shell
apt install ufw

systemctl enable ufw

systemctl start ufw

ufw status

ufw default allow outgoing

ufw default deny incoming

ufw allow from 172.16.238.5 to any port 22 proto tcp

ufw allow from 172.16.238.5 to any port 80 proto tcp

ufw allow from 172.16.100.0/28 to any port 80 proto tcp

ufw deny 8080

ufw enable

ufw delete deny 8080

ufw delete 5

```