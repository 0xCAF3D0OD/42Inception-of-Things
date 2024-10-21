Vagrant.configure("2") do |config|
  
  config.vm.define "tchappuiS" do |control|
        control.vm.hostname = "tchappuiS"
        config.vm.box = "ubuntu/focal64"
        control.vm.network "public_network", ip: "192.168.56.110"
        control.vm.provider "virtualbox" do |v|
          v.customize ["modifyvm", :id, "--name", "tchappuiS"]
          v.memory = 512
          v.cpus = 1
      end
     # config.vm.provision :shell, :inline => SHELL
     #   [...]
     # SHELL
      #  control.vm.provision "shell", path: REDACTED
    end

    config.vm.define "tchappuiSW" do |control|
        control.vm.hostname = "tchappuiSW"
        config.vm.box = "ubuntu/focal64"
        control.vm.network "public_network", ip: "192.168.56.111"
        control.vm.provider "virtualbox" do |v|
          v.customize ["modifyvm", :id, "--name", "tchappuiSW"]
          v.memory = 512
          v.cpus = 1
      end
     # config.vm.provision "shell", inline: <<-SHELL
      #    [...]
      #SHELL
      #control.vm.provision "shell", path: REDACTED
    end
end
