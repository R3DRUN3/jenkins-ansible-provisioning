VAGRANT_API_VERSION=2

Vagrant.configure(VAGRANT_API_VERSION) do |config|
  

  config.vm.box = "ubuntu/focal64"
  config.vm.define "jenkins_2"
  config.ssh.insert_key = false
  config.vm.network "private_network", ip: "192.168.56.10"

  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "jenkins_provisioning.yaml"
  end
end