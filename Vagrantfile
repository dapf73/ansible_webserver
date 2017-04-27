# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.ssh.insert_key = false


  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  for i in 0..5 do
    config.vm.define "vagrant%s" % i  do |vagrant|
        vagrant.vm.box = "bento/centos-6.8-i386"
        vagrant.vm.network "forwarded_port", guest: 80,  host: 8080+i
        vagrant.vm.network "forwarded_port", guest: 443, host: 8440+i
    end
  end
end
