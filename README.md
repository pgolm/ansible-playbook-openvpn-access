# Playbook: OpenVPN AccessServer 

I use this playbook to setup quickly a openvpn-server with ansible.

Tested with Ubuntu 12.04 x64

## Requirements

* python-passlib (need to crypt the prompted password)

## Run

Set the DigitalOcean Env's like:

```
export DO_CLIENT_ID='DO123' DO_API_KEY='abc123'
```

1. Create a Droplet with the Hostname **ovpn** on DigitalOcean

2. Ìnstall the server with ```ansible-playbook vpn.yml -i inventory```

3. Download the VPN-Profil from **https://server-ip:943**, login with user *openvpn*.

4. Connect with ```openvpn --config client.ovpn```
