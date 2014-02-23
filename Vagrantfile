# Vagrant file in which the virtual machine ready to run docker containers on bootup

box = "ubuntu"
url = "http://files.vagrantup.com/precise64.box"
hostname = "scrapy-gsoc2014-it"
ram = "512"


Vagrant::Config.run do |config|
  # All Vagrant configuration is done here.
  
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = box

  # The url from where the 'conf.vm.box' box will be fetched if it
  # doesn't already exist on the user's system.
  config.vm.box_url = url
  
  # Hostname
  config.vm.host_name = hostname

  # Customization
  config.vm.customize [
        'modifyvm', :id,
        '--name', hostname,
        '--memory', ram
      ]
  
end

