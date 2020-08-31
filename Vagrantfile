Vagrant.configure(2) do |config|
  config.vm.box = "bento/centos-7.8"

  config.vm.define "oc" do |oc|
    oc.vm.network "private_network", ip: "192.168.32.11"
    oc.vm.hostname = "oc"
    oc.vm.provider "oc" do |vb|
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define "cm1" do |cm1|
    cm1.vm.network "private_network", ip: "192.168.32.13"
    cm1.vm.hostname = "cm1"
    cm1.vm.provider "cm1" do |vb|
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define "agent1" do |agent1|
    agent1.vm.network "private_network", ip: "192.168.32.15"
    agent1.vm.hostname = "agent1"
    agent1.vm.provider "agent1" do |vb|
      vb.cpus = 1
      vb.memory = 1024
    end
  end
end
