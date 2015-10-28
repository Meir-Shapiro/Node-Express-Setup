# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "urban/trusty64-node"
  config.vm.box_url = "urban/trusty64-node"
  config.vm.network "private_network", ip: "192.168.22.88"
  config.vm.hostname = "tasks.ltccs.dev"
  config.vm.synced_folder ".", "/vagrant"
  
  config.vm.provider :virtualbox do |vb|

	vb.name = "ltc-tasks"
	vb.customize ["modifyvm", :id, "--memory", 2048]
	vb.customize ["modifyvm", :id, "--cpus", 2]
	vb.customize ["guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 10000]
	vb.customize ["setextradata", :id, "VBoxInternal2/SharedFoldersEnableSymlinksCreate/v-root", "1"]
  end

end
