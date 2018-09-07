User
=========

This roles creates the user `user` on a Debian (based) system. Used for the [provision](https://github.com/oneofftech/provision) setup. The account has direct super user access (through sudo) and it optionally gets password information from a simple, encryped [KeePass database](https://keepass.info/).

This is work in progress and it is prefered to collaborate on it. Please communicate over the issue queue. Every pull request is highly appreciated.

Requirements
------------

None


Role Variables
--------------

```yaml
system_user: ""          # populated from keepass
system_user_password: "" # populated from keepass

system_user_authorized_keys: []
```

Dependencies
------------

None

Example Variables
-----------------

```yaml
system_user_authorized_keys:
  - ssh-ed25519 AAAAC3XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX me@desktop
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: xamanu.essentials }
```

License
-------

MIT

Author Information
------------------

Felix Delattre - https://felix.delattre.de
