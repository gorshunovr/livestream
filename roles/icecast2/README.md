Role Name
=========

icecast2 install

Role Variables
--------------

default variables:
```
icecast_location: Earth
icecast_admin_email: info@linkmeup.ru
icecast_hostname: live.linkmeup.ru
icecast_version: 2.4.4*
icecast_listen_port: 8000
icecast_authentication:
  source_password: "5BuziM39pTvaNj7okyAs"
  relay_password: "WVTsPHaA3cOnWAeclLp6"
  admin_user: "PB7rZH"
  admin_password: "458Z1F4CrT49m7XvFozG"
```

Example Playbook
----------------

    - hosts: servers
      become: yes
      roles:
        - icecast2

Tested on
---------

- Ubuntu 20.04 LTS
- Ubuntu 16.04 LTS
- Ubuntu 18.04 LTS
