Vagrant.configure("2") do |config|

  (1..3).each do |i|
    config.vm.define "vm#{i}" do |node|
      config.vm.box = "bento/ubuntu-22.04"
      config.vm.box_architecture = "arm64"
      config.vm.box_version = "202401.31.0"
      config.vm.network "private_network", type: "dhcp"
      config.vm.provider "vmware_desktop" do |v|
        v.gui = false
        v.linked_clone = true
      end
    end

  end

end
