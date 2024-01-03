# ubuntu22-config

Run command
```
sudo apt-add-repository ppa:ansible/ansible
sudo apt update -y
sudo apt install ansible -y

mkdir -p ~/playbooks/ && cd ~/playbooks/
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/devtools-playbook.yml
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/myapp-playbooks.yml

sudo ansible-playbook devtools-playbook.yml
sudo ansible-playbook myapp-playbook.yml

mkdir -p ~/.vim ~/.vim/autoload ~/.vim/backup ~/.vim/colors ~/.vim/plugged
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/.vimrc --directory-prefix=/
```
