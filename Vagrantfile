Vagrant.configure(2) do |config|

    config.vm.box = "ubuntu/xenial64"

    config.vm.define "mysql" do |db|
        db.vm.network "forwarded_port", guest: 3306, host: 3306
        db.vm.provision "shell", path: "bootstrap.sh"
    end
end