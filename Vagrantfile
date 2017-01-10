# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"
  config.ssh.insert_key = false # we use the insecure default key to simplify things

  config.vm.define "mybox" do |mybox|
    config.vm.network "private_network", ip: "192.168.50.4"
    config.vm.network :forwarded_port, guest: 80, host: 4567
  end

  # Run Ansible from the Vagrant VM
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
