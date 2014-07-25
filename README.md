Freepto-lb
==========

Encrypted GNU/Linux OS (based on Debian Wheezy) wich can be installed on USB flash drive.

Freepto is designed for encrypt your communications (OTR, GPG, SSL), carry your documents in secure way (LUKS) and save your anonymity (TOR, OPENVPN)


For developers: build Freepto
=============================

You need a debian wheezy  and some packages installed:
`aptitude install live-build python git-core debootstrap`

Just clone a repository, edit the configuration file:

 vim config/freepto

and run:

`lb config && lb build`

and you'll find a binary.img file :)

We are also providing a Vagrantfile to create quickly a Freepto development environment
https://github.com/AvANa-BBS/freepto-vagrant


For users: Burn Freepto on a USB
================================

You can download the latest images from
https://download.freepto.mx

Use "dmesg" to identify the usb device:
> $ dmesg

Run make-freepto.sh:
> $ sudo bash makefreepto -h

> $ sudo bash makefreepto -i binary.img -p myS3cr3t#luksp4ssw0rd /dev/sdX


Documentation
=============

Italiano:
* https://we.riseup.net/avana/freepto-docs
* https://www.freepto.mx/

Castellano:
* https://we.riseup.net/avana/freepto-docs-es
* https://www.freepto.mx/es/


Screenshots
============

![](http://www.freepto.mx/static/boot.png)
![](http://www.freepto.mx/static/desktop.png)
