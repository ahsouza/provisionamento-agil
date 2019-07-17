# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

# Structure in ruby ​​containing all the activities that the vagrant should perform represented by the object that I called config

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # config.vm creates an object that describes a virtual machine.
  # I called this vm "testvm" and want to use Ubuntu Trusty
  # I indicated that I want a private IP for this machine
  config.vm.define "testvm" do |testvm|
    testvm.vm.box = "ubuntu/trusty64"
    testvm.vm.network :private_network, ip: "192.168.33.2"
    
    testvm.vm.provision "ansible" do |ansible|
      ansible.playbook = "server.yaml"
      ansible.verbose = "vvv"
    end

  end
  # This block gives me access to the virtual machine provider
  # (VirtualBox)
  # I configured this machine with 2GB of memory
  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--memory", "2048"]
  end
  
end