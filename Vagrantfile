Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

  config.vm.define "local_server" do |ubuntu_minikube|

    config.vm.network "forwarded_port",
      guest: 8001,
      host:  8001,
      auto_correct: true

    config.vm.provider "virtualbox" do |vb|
        vb.name = "Local Server"
        vb.memory = "4096"
        vb.cpus = "2"

    # args = []
    # config.vm.provision "shell",
        # path: "scripts/java.sh",
        # args: args

    # args = []
    # config.vm.provision "shell",
    #     path: "scripts/docker.sh",
    #     args: args

    # args = []
    # config.vm.provision "shell",
    #     path: "scripts/minikube.sh",
    #     args: args

    # args = []
    # config.vm.provision "shell",
    #     path: "scripts/kubectl.sh",
    #     args: args
    end

  end

end