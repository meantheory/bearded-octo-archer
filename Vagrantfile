# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

    config.vm.box = "trusty"
    config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"
    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "go.yml"
    end
    #config.vm.network "forwarded_port", guest: 5000, host: 8080

    # config.vm.provider :virtualbox do |vb|
    #   vb.customize ["modifyvm", :id, "--memory", "2048"]
    # end

end
