# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.network "private_network", ip: "192.168.121.254"
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "site.yml"
  end
end
