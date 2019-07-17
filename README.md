# Orquestration of Machine Virtaul with Vagrant


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



## Setting and Up machines virtual with Vagrant

#### Raise a virtual machine

```sh
vagrant up
```

#### Stop a virtual machine

```sh
vagrant halt
```

#### Access via SSH a virtual machine

```sh
vagrant ssh
```

### 2. Up with Shell-Script
```sh
chmod +x run.sh
./run.sh
```