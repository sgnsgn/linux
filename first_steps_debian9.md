# installation debian (ici Debian 9 « Stretch »)
# maj des sources
# https://wiki.debian.org/fr/SourcesList

`nano /etc/apt/sources.list`

```
deb http://deb.debian.org/debian stretch main
deb-src http://deb.debian.org/debian stretch main

deb http://deb.debian.org/debian stretch-updates main
deb-src http://deb.debian.org/debian stretch-updates main

deb http://security.debian.org/debian-security/ stretch/updates main
deb-src http://security.debian.org/debian-security/ stretch/updates main
```

# update & update

```
apt-get update
apt-get upgrade
```

# install VMware Tools

Selectionner `Menu` `VM` `Install VMware Tools`

# monter le cd
# copier le contenu vers le hdd local
# extraire le fichier tar.gz

```
mount /dev/cdrom /mnt
cp /mnt/VMwareTools-9.2.2-1031360.tar.gz ~
cd ~
tar zxvf VMwareTools-9.2.2-1031360.tar.gz
rm -rf VMwareTools-9.2.2-1031360.tar.gz
cd vmware-tools-distrib/
./vmware-install-pl
```

# splitter ses ecrans
apt-get install terminator

