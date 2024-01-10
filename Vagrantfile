Vagrant.configure("2") do |config|
    config.vm.box_check_update = false
  
    #App server
    config.vm.define "app" do |app|
      app.vm.hostname = "appserver.dwp.com"
      app.vm.box = "bento/ubuntu-22.04"
      app.vm.box_version = "202309.08.0"
    end
  
    #DB server
    config.vm.define "db" do |db|
      db.vm.hostname = "dbserver.dwp.com"
      db.vm.box = "bento/ubuntu-22.04"
      db.vm.box_version = "202309.08.0"
    end
  
    #Mail server
    config.vm.define "mail" do |mail|
      mail.vm.hostname = "mailserver.dwp.com"
      mail.vm.box = "bento/ubuntu-22.04"
      mail.vm.box_version = "202309.08.0"
    end
  
    config.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "1024"
       vb.cpus = 1
    end
  end