## User creation

* This role creates the user `user` on a system.
* This user will be added to the groups: `docker`, `ssh_login` and `sudo`
* The password will be set accordingly to the provided information from a simple, encrypted KeePass database.

#### You can connect directly with

`ssh -p 2222 user@123.456.789.1`

or use an alias in your `.ssh/config` (recommended):

```
Host asososca
  Port 2222
  User  user
  Hostname 123.456.789.1
```
