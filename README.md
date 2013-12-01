# Vagrant et al

## Virtualization software

- [Virtualbox](http://www.virtualbox.org)
- KVM / lxc / Xen / VMWare fusion

## What is vagrant

- [Vagrant](http://www.vagrantup.com)
- [Providers](http://docs.vagrantup.com/v2/providers/index.html)
- [Provisioners](http://docs.vagrantup.com/v2/provisioning/index.html)

## Bulding a Vagrant VM box

- [Veewee](https://github.com/jedi4ever/veewee)
- [Packer](http://www.packer.io)

## Getting started in Vagrant

- [Getting Started](http://docs.vagrantup.com/v2/getting-started/index.html)
- [CLI](http://docs.vagrantup.com/v2/cli/index.html)
- [Prebuilt vagrant boxes](http://www.vagrantbox.es)

### Debian Wheezy amd64 Box

```
mkdir debian
cd debian
vagrant init debian https://dl.dropboxusercontent.com/u/197673519/debian-7.2.0.box
```

### Centos 6 x86_64 Box

```
mkdir centos
cd centos
vagrant init centos http://puppet-vagrant-boxes.puppetlabs.com/centos-64-x64-vbox4210-nocm.box
```

## Provisioning

### Simple provisioner
 - [Shell](http://docs.vagrantup.com/v2/provisioning/shell.html)

### Chef-solo provisioner
 - [chef-solo](http://docs.vagrantup.com/v2/provisioning/chef_solo.html)
 - [rove](http://rove.io/)
 - [librarian](https://github.com/applicationsonline/librarian)
 - [berkshelf](https://github.com/berkshelf/berkshelf)
 - [omnibus](https://github.com/opscode/omnibus-ruby)
 - [chef-omnibus](http://www.opscode.com/chef/install)
 - [vagrant-librarian-chef](https://github.com/jimmycuadra/vagrant-librarian-chef)
 - [Vagrant librarian config options](https://github.com/jimmycuadra/vagrant-librarian-chef/blob/master/lib/vagrant-librarian-chef/config.rb)
 - [vagrant-berkshelf](https://github.com/berkshelf/vagrant-berkshelf)
 - [Vagrant berkshelf config options](https://github.com/berkshelf/vagrant-berkshelf/blob/master/lib/berkshelf/vagrant/config.rb)

## Annex

### Vagrant

- [Synced folders](http://docs.vagrantup.com/v2/synced-folders/index.html)
- [Vagrantfile format](http://docs.vagrantup.com/v2/vagrantfile/index.html)
- [Mutli-machine](http://docs.vagrantup.com/v2/multi-machine/index.html)
- [Networking](http://docs.vagrantup.com/v2/networking/index.html)

### Veewee

- [Build Debian Wheezy](http://stacktoheap.com/blog/2013/06/19/building-a-debian-wheezy-vagrant-box-using-veewee/)

### Packer

- [Building with packer](http://blog.codeship.io/2013/11/07/building-vagrant-machines-with-packer.html)