Vagrant::Config.run do |config|
    config.vm.define :service_vm do |inner_config|
        inner_config.vm.box = "base"
        inner_config.vm.forward_port("http", 80, 8080)
        inner_config.vm.forward_port("ssh", 22, 2222)
        inner_config.vm.network("33.33.33.33")

        # this will cause VirtualBox to launch a GUI window for the VM
        #config.vm.boot_mode = :gui
    end
end
