docker
=========

Installs Docker on Linux systems.

Example Playbook
----------------

```
- name: Playbook for Docker installation
  hosts: app
  become: true # Выполнение от имени root
  tasks:
    - name: Ensure apt package list is updated (apt-get update)
      apt: # модуль ansible.builtin.apt
        update_cache: true
        cache_valid_time: 3600

    - name: Ensure Docker is set up
      include_role:
        name: docker
```

Role Variables
--------------

See `defaults/main.yml`.
Available variables to customize:
- docker_required_packages
- docker_packages:
- docker_gpg_key_url
- docker_url
- docker_dist
- docker_version
- docker_user
- docker_services

License
-------

MTI

Author Information
------------------
https://gitlab.com/ansible-roles4162343/ansible-docker#
