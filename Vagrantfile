Vagrant.configure("2") do |config|
  config.vm.define "master" do |vm1|
    vm1.vm.hostname = "master"
    vm1.vm.box = "ubuntu/focal64"
    vm1.vm.network "private_network", ip: "192.168.33.40"
    
    vm1.vm.provider "virtualbox" do |vb|
      vb.name = "master"
      vb.gui = false
      vb.memory = "1024"
    end

    vm1.vm.provision "shell", run: "always", inline: <<-SHELL
        echo "Hello from the master VM"
    SHELL
  end

  config.vm.define "client-vm" do |vm2|
    vm2.vm.hostname = "client-vm"
    vm2.vm.box = "ubuntu/focal64"
    vm2.vm.network "private_network", ip: "192.168.33.20"
    
    vm2.vm.provider "virtualbox" do |vb|
      vb.name = "client-vm"
      vb.gui = false
      vb.memory = "1024"
    end

    vm2.vm.provision "shell", run: "always", inline: <<-SHELL
        echo "Hello from the Client VM"
    SHELL
  end

  config.vm.define "client-vm2" do |vm3|
    vm3.vm.hostname = "client-vm2"
    vm3.vm.box = "ubuntu/focal64"
    vm3.vm.network "private_network", ip: "192.168.33.30"
    
    vm3.vm.provider "virtualbox" do |vb|
      vb.name = "client-vm2"
      vb.gui = false
      vb.memory = "1024"
    end

    vm3.vm.provision "shell", run: "always", inline: <<-SHELL
        echo "Hello from the Client VM2"
    SHELL
  end
  
end
