# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrant virtual development environment for mateusz.loskot.net

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/wily32"
  config.vm.network :forwarded_port, host: 4000, guest: 4000
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install -y ruby2.2
    gem install jekyll
  SHELL
end
