# ansible2

# create master instance with local key > ssh into it> 
# run ssh-keygen > cat id_rsa.pub >save to git key&ssh > 
# cat id_rsa.pub save in aws console like KEY IMPORT (under key pair)
# after lunch 4 instance like workers, copy public IP and paste to hosts file

# install ansible on instance/local 
  # sudo apt update
  # sudo apt install software-properties-common
  # sudo add-apt-repository --yes --update ppa:ansible/ansible
  # sudo apt install ansible

# make file myfirstplaybook.yaml
# to run ansible-playbook -i hosts myfirstplaybook.yaml

# make file delete-resources.yaml
# to delete ansible-playbook -i hosts delete_resources.yaml

# clone all to git repo 

# to check 
# ansible all -i hosts -m command -a "apache2 -v"
# ansible all -i hosts -m command -a "which apache2ctl"
# ansible all -i hosts -m command -a "which apachectl"
