# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANT_API_VERSION = "2"

Vagrant.configure(VAGRANT_API_VERSION) do |config|
  config.vm.box = "ubuntu/xenial64"
  config.ssh.insert_key = false
  config.vm.provider :virtualbox do |v|
    v.memory = 1024
    v.linked_clone = true
  end

  config.vm.define "node1" do |node|
    node.vm.hostname = "node1"
    node.vm.network :private_network, ip: "192.168.60.4"
  end
  config.vm.define "node2" do |node|
    node.vm.hostname = "node2"
    node.vm.network :private_network, ip: "192.168.60.5"
  end
  config.vm.define "node3" do |node|
    node.vm.hostname = "node3"
    node.vm.network :private_network, ip: "192.168.60.6"
  end
end
