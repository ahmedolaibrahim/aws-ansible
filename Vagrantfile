
# -*- mode: ruby -*-
 
# vi: set ft=ruby :

hosts = {
 
  "host1" => "192.168.88.10",
 
  "host2" => "192.168.88.11",
 
  "host3" => "192.168.88.12"
 
}

Vagrant.configure("2") do |config|
 
  config.vm.box = "ubuntu/trusty64"
 hosts.each do |name, ip|
 
    config.vm.define name do |machine|
 
      machine.vm.network :private_network, ip: ip
 
      machine.vm.provider "virtualbox" do |v|
 
        v.name = name
 
      end
 
    end
 
  end
 
end