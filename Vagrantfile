# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "ansible/tower"

    config.vm.define 'ansible' do |ansible|
    ansible.vm.network "private_network", ip: "192.168.10.100"
    ansible.hostsupdater.aliases = ["development.local"]
    ansible.vm.synced_folder "app", "/home/ansible/app"

end
end
