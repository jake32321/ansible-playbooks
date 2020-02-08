# ansible-playbooks
:book: Collection of useful Ansible Playbooks.

## install/configure ansible
For a basic install, Ansible can be installed via ```pip3```. For other installation options please go [here](https://docs.ansible.com/ansible/latest/installation_guide/index.html).
```bash 
pip3 install ansible
```

## configure ansible hosts 
If installed via a package manager you _may_ need to create this file and folder(s).
```bash
/etc/ansible/hosts
```
Add your hosts to ```/etc/ansible/hosts```. These can be added to a group or individually. For a more complete guide for configuring ansible hosts, groups, etc., go [here](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html).
```bash 
sudo vi /etc/ansible/hosts
```

```bash
# /etc/ansible/hosts
[<group_name>]
hostname_one
hostname_two
...
```

## run a playbook 
To execute an Ansible playbook you can simply run:
```bash 
ansible-playbook <playbook_name>.yml
```