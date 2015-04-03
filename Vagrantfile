# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box      = 'packer-debian'
  config.vm.box_url  = 'debian-wheezy-64.box'

  config.vm.provider :virtualbox do |vb|
    vb.customize ['modifyvm', :id, '--ostype', 'Debian_64']
    vb.customize ['modifyvm', :id, '--memory', 1024]
    vb.customize ['modifyvm', :id, '--chipset', 'ich9']
    vb.customize ['modifyvm', :id, '--vram', '10']
    vb.customize ['modifyvm', :id, '--ioapic', 'on']
    vb.customize ['modifyvm', :id, '--cpus', 2]
  end
end
