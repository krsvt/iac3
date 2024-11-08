# Lab 2

## Up VMs
```
vagrant up
```
## Install docker role
Docker role in Gitlab: https://gitlab.com/ansible-roles4162343/ansible-docker#
```
ansible-galaxy install -r requirements.yml
```
```
*[master][~/dev/itmo/infra/lab2]$ ansible-galaxy list

# /home/svt/.ansible/roles
- docker, master
[WARNING]: - the configured path /usr/share/ansible/roles does not exist.
[WARNING]: - the configured path /etc/ansible/roles does not exist.
```

## Run playbook
```
ansible-playbook playbook.yaml -i inventory.ini
```
## Check apps
Port-forwarding:
http://localhost:8001-http://localhost:8003
