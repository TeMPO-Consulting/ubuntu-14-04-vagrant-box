ubuntu-14-04-vagrant-box
========================

Ubuntu Server 14.04 64 Vagrant Box (Docker included)

# Add ubuntu-14-04 box
vagrant box add ubuntu-14-04 https://oss-binaries.phusionpassenger.com/vagrant/boxes/latest/ubuntu-14.04-amd64-vbox.box

# Edit Vagrantfile
set your host share folder on any other dir you want (than ../../vmshared)

guest share folder in: /vagrant_data

config.vm.synced_folder "../../vmshared", "/vagrant_data"

# Start (and provision at 1st up)
vagrant up

vagrant ssh

# Stop
exit

vagrant halt

# Provision (after 1st up)
vagrant up

vagrant provision
