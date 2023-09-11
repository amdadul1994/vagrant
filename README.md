vagrant box add ubuntu/focal64 --add local machine a image
vagrant init ubuntu/focal64 ------------------create vagrant file
vagrant plugin install vagrant-vbguest ---- install plugin
vagrant up ------------ start machine
vagrant ssh -------------------------ssh to machine
vagrant halt --------------------------shutdown the machine
vagrant destroy -------------------delete the machine
vagrant validate ------------------validate the vagrant file
vagrant status ------------------------check the vagrant machine status

when multiple machines start at the same vagrant file:
vagrant validate machine-name
vagrant ssh machine-name
vagrant up machine-name

