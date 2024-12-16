# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/rhel8"

  config.vm.network "public_network"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.name = "Tortoise"
    vb.cpus = 4
    vb.memory = 4096
    vb.linked_clone = true
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.raw_arguments = ["--extra-vars", "@credentials.yml"]
  end
end
