# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  config.vm.provision "shell", privileged: false, inline: <<-SHELL
  	curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash
		cd /vagrant
		chmod u+x build.sh
		./build.sh
	SHELL
end
