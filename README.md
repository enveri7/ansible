#Vagrantbox + ansible provisioning

###Ubuntu 12.04 LTS (precise64)
###Release:	12.04
###php5 + apache2

###Just do vagrant up and vagrant ssh.

##Install ansible
###http://docs.ansible.com/ansible/intro_installation.html

##To reboot vagrant server and run ansible playbook
###vagrant reload --provision

##Just to run ansible playbook
###ansible-playbook playbook.yml

##To see ansible tasks
###ansible-playbook playbook.yml --list-tasks
