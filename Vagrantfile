# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/jammy64"

  # VM1 configuration
  config.vm.define "vm1" do |vm1|
    vm1.vm.network "private_network", ip: "192.168.56.2"
    vm1.vm.hostname = "vm1"
    vm1.vm.provider "virtualbox" do |vb|
      vb.name = "vm1"
      vb.memory = "1024"
      vb.cpus = 2
    end
  end

  # VM2 configuration
  config.vm.define "vm2" do |vm2|
    vm2.vm.network "private_network", ip: "192.168.56.3"
    vm2.vm.hostname = "vm2"
    vm2.vm.provider "virtualbox" do |vb|
      vb.name = "vm2"
      vb.memory = "1024"
      vb.cpus = 2
    end
  end

  # VM3 configuration
  config.vm.define "vm3" do |vm3|
    vm3.vm.network "private_network", ip: "192.168.56.4"
    vm3.vm.hostname = "vm3"
    vm3.vm.provider "virtualbox" do |vb|
      vb.name = "vm3"
      vb.memory = "1024"
      vb.cpus = 2
    end
  end

  # Ansible provisioning 
  # config.vm.provision "ansible" do |ansible|
  #   ansible.playbook = "playbook.yml"
  #   ansible.inventory_path = "inventory.ini"
  # end

end
