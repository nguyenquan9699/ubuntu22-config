# ubuntu22-config

## Install ansible
```
sudo apt-add-repository ppa:ansible/ansible
sudo apt update -y
sudo apt install ansible -y
```
## Install & Config Development Tools & Apps

```
mkdir -p ~/playbooks/
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/devtools-playbook.yml --directory-prefix=~/playbooks/
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/general-apps-playbooks.yml  --directory-prefix=~/playbooks/
mkdir -p ~/.vim ~/.vim/autoload ~/.vim/backup ~/.vim/colors ~/.vim/plugged
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/.vimrc --directory-prefix=~/


sudo ansible-playbook ~/playbooks/devtools-playbook.yml
sudo ansible-playbook ~/playbooks/general-apps-playbooks.yml
```

## Install DevOps Tools

```
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/devops-tools-playbook.yml  --directory-prefix=~/playbooks/

sudo ansible-playbook ~/playbooks/devops-tools-playbook.yml
```

## Install Monitor Server Tools
```
wget https://raw.githubusercontent.com/nguyenquan9699/ubuntu22-config/main/monitor-server.yml  --directory-prefix=~/playbooks/

sudo ansible-playbook ~/playbooks/monitor-server.yml

```