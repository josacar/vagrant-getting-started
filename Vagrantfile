# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Shell provisioner
  $script = <<-SCRIPT
  echo Provisining a machine in valencia.rb...
  date > /etc/vagrant_provisioned_at
  SCRIPT

  # config.vm.provision "shell", inline: "echo Hello"
  # config.vm.provision "shell", $script
  config.vm.provision "shell", path: "script.sh"

  config.omnibus.chef_version = "10.28.2"
  # config.berkshelf.enabled = true
  # Chef-solo provisioner
  # config.vm.provision :chef_solo do |chef|
  #   chef.cookbooks_path = ["cookbooks"]
  #   chef.add_recipe 'apt'
  #   chef.add_recipe 'rbenv::user'
  #   chef.roles_path = "roles"
  #   chef.data_bags_path = "data_bags"
  #   chef.add_recipe "mysql"
  #   chef.add_role "web"
  #   chef.json = { :mysql_password => "foo" }
  # end

  # config.vm.network :forwarded_port, guest: 80, host: 8080
  # config.vm.network :private_network, ip: "192.168.33.10"
  # config.vm.network :public_network
  # config.ssh.forward_agent = true
  # config.ssh.forward_x11 = true
  # config.vm.synced_folder ".", "/vagrant", :nfs => true
  # config.vm.provider :virtualbox do |vb|
  #   vb.gui = true
  #   vb.customize ["modifyvm", :id, "--memory", "1024"]
  # end
  #
  config.vm.define 'debian' do  |config|
    config.vm.provider :virtualbox
    config.vm.box = 'debian'
    config.vm.box_url = "https://dl.dropboxusercontent.com/u/197673519/debian-7.2.0.box"
    config.vm.network "private_network", ip: "192.168.50.4"
  end

  config.vm.define 'centos' do  |config|
    config.vm.provider :virtualbox
    config.vm.box = "centos"
    config.vm.box_url = "http://puppet-vagrant-boxes.puppetlabs.com/centos-64-x64-vbox4210-nocm.box"
    config.vm.network "private_network", ip: "192.168.50.5"
  end
end