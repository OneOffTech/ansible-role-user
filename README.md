User
=========

This roles creates the user `user` on a Debian (based) system. Used for the [provision](https://github.com/oneofftech/provision) setup. The account has direct super user access (through sudo) and it optionally gets password information from a simple, encryped [KeePass databse](https://keepass.info/).

This is work in progress and it is prefered to collaborate on it. Please communicate over the issue queue. Every pull request is highly appreciated.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: xamanu.essentials }

License
-------

MIT

Author Information
------------------

Felix Delattre - https://felix.delattre.de
