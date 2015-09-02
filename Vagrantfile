# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.provision :shell, path: "install.sh", args: "ubuntu 1404 desktop mosrs"
  config.ssh.forward_x11 = true

  config.vm.provider "virtualbox" do |v|
    v.gui = true
    v.memory = 1024
    v.cpus = 2
  end

end