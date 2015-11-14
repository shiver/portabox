Portabox
--------

Portable, ephemeral, minimal development desktop.

**Disclaimer:** This is primarily intended for personal use and likely a constant work-in-progress.

Requirements
------------

* vagrant
* virtualbox

Vagrant Plugins:
* vagrant-hostmanager
* vagrant-guest_ansible

Installation
------------

Install the required Vagrant plugins:
```
$ vagrant plugin install vagrant-hostmanager vagrant-guest_ansible
```

Provision the virtual machine:
```
$ git clone https://github.com/shiver/portabox.git
$ vagrant up
```
