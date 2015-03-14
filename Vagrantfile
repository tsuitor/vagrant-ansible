# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  
  config.vm.box = "parallels/ubuntu-14.04"

  config.vm.network "forwarded_port", guest: 80, host: 8088

  config.vm.provision :ansible do |ansible| 
    ansible.playbook = "playbook.yml"
  end
  
end
