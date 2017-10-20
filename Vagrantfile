# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
	config.vm.define "master" do |master|
  	master.vm.box = "centos/7"
		master.vm.network :public_network
		master.vm.synced_folder ".", "/vagrant", disabled: true
		#master.vm.provider "virtualbox" do |v|
		#	v.customize ["modifyvm", :id, "--cpuexecutioncap", "100", "--memory", "1024"]
		#end
	end
	config.vm.define "node" do |node|
  	node.vm.box = "centos/7"
		node.vm.network :public_network
		node.vm.synced_folder ".", "/vagrant", disabled: true
		#node.vm.provider "virtualbox" do |v|
		#	v.customize ["modifyvm", :id, "--cpuexecutioncap", "100", "--memory", "1024"]
		#end
	end
end
