# Lab 3

## Up VMs
```
vagrant up
```
## Install roles

docker role in Gitlab: https://gitlab.com/ansible-roles4162343/ansible-docker#

nginx role in Gitlab: https://gitlab.com/ansible-roles4162343/ansible-nginx#
```
ansible-galaxy install -r requirements.yml
```

## Run playbook
```
ansible-playbook playbook.yaml -i inventory.ini
```
## Check apps
Port-forwarding:
http://localhost:8001 - srv1, application 

http://localhost:8002 - srv2, application 

http://localhost:8003 (http://localhost:8003/catalog) - srv3, nginx 
