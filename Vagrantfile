# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.box_check_update = false
  config.vm.hostname = "testing"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.network  "forwarded_port", guest: 8888, host: 9999
  config.vm.define "testing"
  config.vm.provider "virtualbox" do |vb|
     vb.gui = false
     vb.memory = "1024"
  end
end
