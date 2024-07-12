Vagrant.configure("2") do |config|
 
 #Define the first VM
 config.vm.define "vm1" do |vm1|
  vm1.vm.box = "bento/ubuntu-22.04"
  vm1.vm.hostname = "master"
  vm1.vm.network "private_network", ip: "192.168.56.11"
  vm1.vm.network "public_network", bridge: "wlp3s0"
  vm1.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
  end
 end

 #Define the second VM
 config.vm.define "vm2" do |vm2|
  vm2.vm.box = "bento/ubuntu-22.04"
  vm2.vm.hostname = "worker1"
  vm2.vm.network "private_network", ip: "192.168.56.12"
  vm2.vm.network "public_network", bridge: "wlp3s0"
  vm2.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end
 end

 #Define the third VM
 config.vm.define "vm3" do |vm3|
  vm3.vm.box = "bento/ubuntu-22.04"
  vm3.vm.hostname = "worker2"
  vm3.vm.network "private_network", ip: "192.168.56.13"
  vm3.vm.network "public_network", bridge: "wlp3s0"
  vm3.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end
 end

end
