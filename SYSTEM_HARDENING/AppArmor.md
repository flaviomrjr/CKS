AppArmor
========

systemctl status apparmor

cat /sys/module/apparmor/parameter/enabled

cat /sys/kernel/security/apparmor/profiles

aa-status

## Creating AppArmor Profiles

apt-get install -y apparmor-utils

aa-genprof

Load a profile:

apparmor_parser /etc/apparmor.d/root.add_data.sh

Disable the profile
apparmor_parser -R /etc/apparmos.d/root.add_data.sh

## AppArmor in K8S


