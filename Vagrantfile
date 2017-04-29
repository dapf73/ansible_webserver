# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.ssh.insert_key = false
  config.vm.provider "virtualbox" do |v|
    v.memory = 256
    v.cpus   = 1
  end

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  config.vm.define "ws0"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8080
      vagrant.vm.network "forwarded_port", guest: 443, host: 8440
  end
  config.vm.define "ws1"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8081
      vagrant.vm.network "forwarded_port", guest: 443, host: 8441
  end
  config.vm.define "ws2"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8082
      vagrant.vm.network "forwarded_port", guest: 443, host: 8442
  end
  config.vm.define "ws3"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8083
      vagrant.vm.network "forwarded_port", guest: 443, host: 8443
  end
  config.vm.define "ws4"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8084
      vagrant.vm.network "forwarded_port", guest: 443, host: 8444
  end
  config.vm.define "ws5"  do |vagrant|
      vagrant.vm.box = "bento/centos-6.8-i386"
      vagrant.vm.network "forwarded_port", guest: 80,  host: 8085
      vagrant.vm.network "forwarded_port", guest: 443, host: 8445
  end
end
