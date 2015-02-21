# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  
  config.vm.network "private_network", ip: "192.168.50.4"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
  end

  config.vm.define "dev01" do |machine|
    machine.vm.hostname = "dev01"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.groups = {
      "nexus.development" => ["dev01"]
    }
    ansible.playbook = "nexus.yml"
  end
end
