Role ts
=========

Linkmeup live broadcast server install role.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml).

Prerequisites
-------------

Ubuntu 18.04 VM with Gnome 3 desktop and Sound card.

Example Playbook
----------------

    - hosts: ts
      tasks:
        - include_role:
            name: ts
          vars:
            icecast_address: live.linkmeup.ru
            icecast_password: "5BuziM39pTvaNj7okyAs"

License
-------

MIT.

Author Information
------------------

Roman Gorshunov, linkmeup project, 2020
