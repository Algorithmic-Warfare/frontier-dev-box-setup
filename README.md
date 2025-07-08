# frontier-dev-box-setup
An Ansible script for setting up dev boxes for Frontier MUD/Assembly programming.

## How to setup

Ensure your system is up-to-date:
```bash
sudo apt update
sudo apt upgrade -y
```

Reboot the system if necessary:
```bash
sudo reboot
Step 2: Add Ansible PPA Repository
```

To get the latest version of Ansible, add its official PPA:
```bash
sudo apt install -y software-properties-common
sudo add-apt-repository --yes --update ppa:ansible/ansible
```

Update the package index:
```bash
sudo apt update
```

Install Ansible using the following command:
```bash
sudo apt install -y ansible
```

Verify the installation:
```bash
ansible --version
```

## How to run

```bash
ansible-playbook -i inventory.ini playbook.yml --ask-become-pass
```
