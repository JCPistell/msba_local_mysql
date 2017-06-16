Vagrant.configure("2") do |config|
    config.vm.define "mysql" do |mysql|
        mysql.vm.box = "ubuntu/trusty64"
        mysql.vm.network "private_network", ip: "192.168.56.101"
        mysql.vm.provider "virtualbox" do |vb|
            vb.memory = "2048"
        end
        mysql.vm.provision "shell", path: "provisionDB.sh"
    end
end

