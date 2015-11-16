Vagrant.configure(2) do |config|
    config.hostmanager.enabled = true
    config.hostmanager.manage_host = true

    config.vm.define "portabox" do |portabox|
        portabox.vm.hostname = "portabox"
        portabox.vm.box = "ubuntu/trusty64"
        portabox.vm.network "private_network", ip: "192.168.33.10"
        portabox.vm.synced_folder File.expand_path("~"), "/home/vagrant/host"

        portabox.vm.provider "virtualbox" do |provider|
            provider.name = "portabox"
            provider.gui = true
            provider.memory = "1024"
        end

        # Replace with ansible_local when Vagrant 2.0 is released
        portabox.vm.provision :guest_ansible do |ansible|
            ansible.playbook = "playbook.yml"
        end
    end
end
