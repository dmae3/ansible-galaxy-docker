Docker install role
=========

Docker install ansible galaxy role.

Requirements
------------

None

Role Variables
--------------

* docker_version  
Install Docker version

* docker_users  
If you need join users to docker group.  
Set this.  
```yml
docker_users:
  - user1
  - user2
```

Dependencies
------------

None

Example Playbook
----------------

```yml
---
- hosts: all
  become: true
  roles:
    - role: galaxy-docker
      docker_users:
        - user1
        - user2
```

License
-------

BSD

Author Information
------------------

[Daisuke Maeda](https://github.com/dmae3 "Daisuke Maeda")
