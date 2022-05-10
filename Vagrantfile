Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/trusty64"

    config.vm.provider "virtualbox" do |v|
        v.memory = 1024
    end

    config.vm.define "wordpress" do |m|
        m.vm.network "public_network", bridge: "enp8s0", ip: "192.168.1.102"
    end

    config.vm.define "mysql" do |m|
        m.vm.network "public_network", bridge: "enp8s0", ip: "192.168.1.103"
    end

end