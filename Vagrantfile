# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "centos7"
  config.vm.box_url = "https://dl.dropboxusercontent.com/u/98748673/centos7.box"

  config.vm.network :forwarded_port, guest: 3000, host: 3000, protocol: 'tcp'
  config.vm.network :forwarded_port, guest: 3306, host: 3306, protocol: 'tcp'

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
    vb.memory = "1024"
  end

end
