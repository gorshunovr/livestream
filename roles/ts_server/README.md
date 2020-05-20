Ts Server Role
==============

install and configure packages:
  - darkice
  - pulseaudio
  - xfce4
  - xfce4-goodies
  - tigervnc-standalone-server
  - audacious

Role Variables
--------------

default variables:
```
linkmeup_vnc_password: "ThJ48Dp4gprIhd8"
icecast_listen_port: 8000
icecast_hostname: live.linkmeup.ru
icecast_authentication:
  source_password: "5BuziM39pTvaNj7okyAs"
darkice:
  mount_point: live
  name: "Подкаст linkmeup"
  description: "Прямой эфир подкаста linkmeup"
  url: https://linkmeup.ru
  dump_file: dump.mp3
```

Dependencies
------------

  icecast2 role

Example Playbook
----------------

    - hosts: servers
      become: yes
      roles:
         - ts_server

Tested on
---------

  - Ubuntu 18.04 LTS
  - Ubuntu 20.04 LTS
