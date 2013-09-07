Vagrant::Config.run do |config|

  config.vm.box = "precise32"
  config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.forward_port 8124, 8124
  config.vm.provision :shell,
    :inline => "sudo apt-get update && sudo apt-get -y install build-essential git ruby1.9.3 && sudo gem install github-pages --no-ri --no-rdoc"

  config.ssh.forward_agent = true
end
