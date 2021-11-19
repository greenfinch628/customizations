# -*- mode: ruby -*-
# vi: set ft=ruby :
#
 VAGRANTFILE_API_VERSION = "2"

 Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
	config.vm.box = "geerlingguy/centos8"
	config.ssh.insert_key = false
	config.vm.synced_folder ".", "/vagrant", disabled: false
	
	config.vm.provider :virtualbox do |vb|
		vb.memory = 1024
	end
	
	config.vm.define "centos08-01" do |centos8|
		centos8.vm.hostname = "centos08-01.test"
		centos8.vm.network :private_network, ip: "192.168.60.8"
	end

	#config.vm.provision :ansible do |ansible|
	#	ansible.playbook = "main-setting.yml"
	#end
 end
