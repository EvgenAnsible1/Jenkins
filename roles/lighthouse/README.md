Role Name
=========

Netology 8.4 homrework lighthouse role

Requirements
------------

Role include nginx server installation.

Role Variables
--------------
F: You can change download URL.
```yaml
lighthouse_git: https://github.com/vkcom/lighthouse
```
F: You can cange location directory.
```yaml
lighthouse_dir: /home/student/lighthouse
```
F: You can change nginx user name.
```yaml
nginx_user: root
```

Dependencies
------------

-

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role }

License
-------

MIT

Author Information
------------------

Evgeniy Smirnov
