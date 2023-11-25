#$default_network_interface = `ip route | awk '/^default/ {printf "%s", $5; exit 0}'`


Vagrant.configure("2") do |config|   #copiar la config minima del repo vagrant boxes
 config.vm.define "devops" do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "devops"
  #config.vm.network "private_network", bridge: "#$default_network_interface", ip:"192.168.5.187"  
  config.vm.network "public_network", ip:"192.168.5.187"  
  config.vm.provider "virtualbox" do |vmsetup|
  vmsetup.memory = 512
  vmsetup.cpus = 1
  end  
 end
end


Vagrant.configure("2") do |config|   #copiar la config minima del repo vagrant boxes
  config.vm.define "devops-2" do |config|
   config.vm.box = "ubuntu/xenial64"
   config.vm.hostname = "devops-2"
   #config.vm.network "private_network", bridge: "#$default_network_interface", ip:"192.168.5.187"  
   config.vm.network "public_network", ip:"192.168.5.188"  
   config.vm.provider "virtualbox" do |vmsetup|
   vmsetup.memory = 512
   vmsetup.cpus = 1
   end  
  end
 end