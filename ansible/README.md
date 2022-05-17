# Ansible configurations

Guidance to ansible configuration and different steps.

## Install and configure ansible on master node

- Apply following steps to install correct version of ansible on master node:

```
sudo apt update
sudo apt install python3-pip python3-dev
python3 -m pip install -U pip
python3 -m pip install --user ansible==5.6.0
ansible-galaxy install -r roles/requirements.yml
```

- Generate ssh key for ubuntu user on gateway:

```
ssh-keygen
```

- Copy public key to main repository deploy keys to have access to the project.

- Pull main project from github and configure webhook runner on master node.
