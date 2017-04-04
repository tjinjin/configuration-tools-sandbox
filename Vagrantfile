# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.ssh.insert_key = false

  config.vm.define :centos do |centos|
    centos.vm.box = "bento/centos-7.2"
    centos.vm.network "private_network", ip: "192.168.33.10"
    centos.cache.scope = :box if Vagrant.has_plugin? 'vagrant-cachier'
  end

  config.vm.define :ubuntu do |ubuntu|
    ubuntu.vm.box = "ubuntu/trusty64"
    ubuntu.vm.network "private_network", ip: "192.168.33.11"
    ubuntu.cache.scope = :box if Vagrant.has_plugin? 'vagrant-cachier'
  end
end
