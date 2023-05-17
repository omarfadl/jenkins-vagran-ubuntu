Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.network "public_network"
  
  config.vm.provider "virtualbox" do |vb|
    vb.name="jenkins"
    vb.gui = false
    vb.cpus = 2
    vb.memory = "4096"
  end
  
  config.vm.provision "shell" do |shell|
    shell.path = "jenkins.sh"
  end
end
