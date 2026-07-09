---
description: For Ubuntu 22.04, 20.04 and 18.04
---

# Connecting VM to the Internet.

Go to /etc/netplan and make a file called 1-netcfg.yaml



```
network:
  version: 2
  renderer: networkd
  ethernets:
    eth0:
      dhcp4: no
      dhcp6: no
      addresses:
        - address/32
      nameservers:
        addresses:
          - 208.67.222.222
          - 208.67.220.220
      routes:
          - to: 0.0.0.0/0
            via: 144.217.253.254
            on-link: true
      match:
        macaddress: maddress
```

Change the address to the VPS IP

Change the maddress to the Mac Address.&#x20;

then do&#x20;

```
sudo ip link set eth0 down
run the cmd again but with up
sudo ip link set eth0 up

sudo netplan apply 

sudo systemctl restart systemd-networkd

Then test by pinging 8.8.8.8

ping 8.8.8.8

and you should get traffic
```

