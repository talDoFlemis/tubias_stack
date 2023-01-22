# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define :nginx do |nginx|
    nginx.vm.network :private_network, ip: "7.7.7.2"
  end

  config.vm.define :tomcat do |tomcat|
    tomcat.vm.network :private_network, ip: "7.7.7.3"
  end

  config.vm.define :mq do |mq|
    mq.vm.network :private_network, ip: "7.7.7.4"
  end

  config.vm.define :cache do |cache|
    cache.vm.network :private_network, ip: "7.7.7.5"
  end

  config.vm.define :sql do |sql|
    cache.vm.network :private_network, ip: "7.7.7.6"
  end

  config.vm.provider :libvirt do |lv|
    lv.default_prefix = 'tubias'
  end
end
