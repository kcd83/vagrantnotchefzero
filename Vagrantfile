# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "chef/centos-6.5"

  config.vm.provision "chef_zero" do |chef|
    chef.environments_path = "environments"
    chef.environment = "testenv"
  #   chef.add_recipe "yum"
  end
end
