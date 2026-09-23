Vagrant.configure("2") do |config|

  config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.define "web01" do |web01|
    web01.vm.box = "nobreak-labs/rocky-10"
    web01.vm.hostname = "web01"
    web01.vm.network "private_network", ip: "192.168.56.20", auto_config: false
    web01.vm.network "private_network", ip: "10.10.10.11", auto_config: false
    web01.vm.network "private_network", ip: "10.10.20.11", auto_config: false
    web01.vm.disk :disk, size: "5GB", name: "extra_disk"
    web01.vm.provider "virtualbox" do |vb|
      vb.name = "web01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "was01" do |was01|
    was01.vm.box = "nobreak-labs/rocky-10"
    was01.vm.hostname = "was01"
    was01.vm.network "private_network", ip: "192.168.56.21", auto_config: false
    was01.vm.network "private_network", ip: "10.10.10.12", auto_config: false
    was01.vm.network "private_network", ip: "10.10.20.12", auto_config: false
    was01.vm.provider "virtualbox" do |vb|
      vb.name = "was01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "db01" do |db01|
    db01.vm.box = "nobreak-labs/rocky-10"
    db01.vm.hostname = "db01"
    db01.vm.network "private_network", ip: "192.168.56.22", auto_config: false
    db01.vm.network "private_network", ip: "10.10.10.13", auto_config: false
    db01.vm.network "private_network", ip: "10.10.20.13", auto_config: false
    db01.vm.provider "virtualbox" do |vb|
      vb.name = "db01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "monitor01" do |monitor01|
    monitor01.vm.box = "nobreak-labs/rocky-10"
    monitor01.vm.hostname = "monitor01"
    monitor01.vm.network "private_network", ip: "192.168.56.23", auto_config: false
    monitor01.vm.network "private_network", ip: "10.10.10.14", auto_config: false
    monitor01.vm.provider "virtualbox" do |vb|
      vb.name = "monitor01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "web02" do |web02|
    web02.vm.box = "nobreak-labs/rocky-10"
    web02.vm.hostname = "web02"
    web02.vm.network "private_network", ip: "192.168.56.24", auto_config: false
    web02.vm.network "private_network", ip: "10.10.10.15", auto_config: false
    web02.vm.network "private_network", ip: "10.10.20.15", auto_config: false
    web02.vm.provider "virtualbox" do |vb|
      vb.name = "web02"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  config.vm.define "lb01" do |lb01|
    lb01.vm.box = "nobreak-labs/rocky-10"
    lb01.vm.hostname = "lb01"
    lb01.vm.network "private_network", ip: "192.168.56.25", auto_config: false
    lb01.vm.network "private_network", ip: "10.10.10.16", auto_config: false
    lb01.vm.provider "virtualbox" do |vb|
      vb.name = "lb01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

end
