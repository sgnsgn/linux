# bind9 (DNS)

http://powtos.fr/1003-mise-en-place-bind9-debian-7/

https://www.supinfo.com/articles/single/1709-mise-place-serveur-dns-avec-bind9

https://www.supinfo.com/articles/single/1714-mise-place-serveurs-dns-maitre-esclave-avec-bind9

https://www.supinfo.com/articles/single/1715-dynamic-dns-avec-bind9-isc-dhcp-server


# dhcp

https://openclassrooms.com/courses/mise-en-place-d-un-serveur-dhcp-sous-linux

# divers

https://github.com/shad0wuser

http://www.installerunserveur.com/

# installations des paquets bind9 (dns) / isc-dhcp / terminator (split console)

```bash
apt-get install bind9 bind9utils bind9-doc dnsutils isc-dhcp-server git terminator
```

# For eth0 with dhcp:

# The loopback network interface
`auto lo eth0`
`iface lo inet loopback`

# The primary network interface
`iface eth0 inet dhcp
For eth0 static:`

# The loopback network interface
`auto lo eth0
iface lo inet loopback`

# The primary network interface
```iface eth0 inet static
    address 192.168.10.33
    netmask 255.255.255.0
    broadcast 192.168.10.255
    network 192.168.10.0
    gateway 192.168.10.254 
dns-nameservers 192.168.10.254
```

# commandes en vrac

```
dhclient ens33
ifup ens33
ifdown ens33
ifconfig eth0
```

