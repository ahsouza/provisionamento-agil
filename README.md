# Orquestration of Machine Virtaul with Vagrant

### Vagrant currently supports the following providers

* VirtualBox
* Hyper-V
* VMWARE
* KVM
* Azure
* AWS
* Google
* digitalocean
* proxmox
* Openstack
* Docker

## Installing VirtualBox Oracle

### Download VirtualBox v.5.2

```sh
wget -c https://download.virtualbox.org/virtualbox/5.2.20/VirtualBox-5.2.20-125813-Linux_amd64.run -O virtualbox.run
```

### Permissao de execução

```sh
chmod +x virtualbox.run
```

### Exec file with sudo

```sh
sudo ./virtualbox.run
```



## Commands Vagrant

#### Raise a virtual machine

```sh
vagrant up
```

#### Stop a virtual machine

```sh
vagrant halt
```

#### Destroy a virtual machine

```sh
vagrant destroy
```

#### Access via SSH a virtual machine

```sh
vagrant ssh
```

#### Run only the shell script provisioning driver

```sh
vagrant provision
```