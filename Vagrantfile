# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.network "private_network", ip: "192.168.10.254"
  config.vm.network :forwarded_port, guest: 22, host: 2222
  config.vm.network :forwarded_port, guest: 80, host: 80
  config.vm.network :forwarded_port, guest: 443, host: 443
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "site.yml"
  end
end
