Portabox
--------

Portable, ephemeral, minimal development desktop.

Requirements
------------

* vagrant
* virtualbox

Vagrant Plugins:
* hostmanager
* vagrant-guest_ansible

Installation
------------

Install the required Vagrant plugins:
```
$ vagrant plugin install hostmanager vagrant-guest_ansible
```

Provision the virtual machine:
```
$ git clone https://github.com/shiver/portabox.git
$ vagrant up
```
