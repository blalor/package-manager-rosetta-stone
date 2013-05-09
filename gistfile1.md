```
fedora              debian
rpm -i foo.rpm      dpkg -i foo.deb
rpm -e foo          dpkg -P foo
rpm -qip foo.rpm    dpkg -I foo.deb
rpm -qlp foo.rpm    dpkg -c foo.deb
rpm -ql foo         dpkg -L foo
rpm -qi foo         dpkg -p foo, dpkg -s foo
rpm -qa             dpkg-query -W, dpkg --list
yum list installed  dpkg-query -W, dpkg --list
rpm -qf /bin/bash   dpkg -S /bin/bash

yum install foo     apt-get install foo

yum search foo      apt-cache search foo
yum info foo        apt-cache show foo
yum list available  apt-cache dumpavail

rpm2cpio bash.rpm | cpio -diu   dpkg -x bash.deb $PWD
```




http://cupcakecarnival.net/2009/02/17/debian-equivalent-rpm-based-system-commands
http://wiki.debian.org/RPM
https://help.ubuntu.com/community/SwitchingToUbuntu/FromLinux/RedHatEnterpriseLinuxAndFedora
