Vagrant.configure('2') do |config|
  config.vm.box = 'osx'

  config.vm.provider 'vmware_fusion' do |v|
    v.vmx['ethernet0.virtualDev'] = 'e1000' # Fix networking: https://groups.google.com/d/msg/vagrant-up/VyZBqzbVzvs/GzWECRRuSxgJ

    v.gui = true
    v.vmx['memsize'] = '2048'
    v.vmx['numvcpus'] = '1'
    v.vmx['displayName'] = 'Vagrant OSX'
  end
end
