# Playbook: OpenVPN AccessServer 

I use this playbook to setup quickly a openvpn-server with ansible.

Tested with Ubuntu 12.04 x64

## Requirements

* python-passlib (need to crypt the prompted password)

## Run

```bash
ANSIBLE_HOSTS=<server-ip>, ansible-playbook vpn.yml
```

Download the VPN-Profil from **https://server-ip:943**, login with user *openvpn*.
