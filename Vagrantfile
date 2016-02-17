# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  config.vm.box = "teknology/rush-box-32bit"
  config.vm.provision :shell, :path => "bootstrap.sh"
  config.vm.provision :shell, :path => "toolsprovision.sh", privileged:false
  config.vm.network "private_network", ip: "192.168.33.43"
  config.vm.hostname = "local.rushbox.com"
  #config.hostsupdater.aliases = ["local.vanitycurls.com"]

  #Allows for connecting to the vagrant box with an external mysql client
  config.vm.network "forwarded_port", guest: 3306, host: 3306
  config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]


end
