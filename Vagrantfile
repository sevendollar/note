Vagrant.configure("2") do |config|
  config.vm.box = 'vsphere-dummybox'
  config.ssh.username = 'ubuntu'
  config.ssh.private_key_path = '/home/ubuntu/.ssh/key'
  config.ssh.insert_key = false

  config.vm.provider :vsphere do |vsphere|
    vsphere.host = '192.168.15.195'
    vsphere.data_center_name = 'taiping'
    vsphere.compute_resource_name = 'dell'
    vsphere.resource_pool_name = 'vagrant'
    vsphere.template_name = 'vagrant-templates/base-vagrant-ubuntu-wily'
    vsphere.vm_base_path = 'vagrant-templates'
    vsphere.notes = 'Vagrant created VM.'
    vsphere.user = ''
    vsphere.password = ''
    vsphere.insecure = true
    vsphere.linked_clone = true
    vsphere.memory_mb = '512'
    vsphere.cpu_count = '1'
  end
end
