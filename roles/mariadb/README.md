# Ansible Role: MariaDB

Installs MariaDB

## Supported platforms

```
Ubuntu 16.04
```

## Post install

Run `mysql_secure_installation`

## Requirements

None

## Role Variables

MariaDB version:

```
mariadb_version: 10.1
```


### Experimental unattended mysql_secure_installation

```
ansible-playbook release.yml --extra-vars "mysql_secure_installation=true mysql_root_password=your_very_secret_password"
```

## Dependencies

None

## Example Playbook

```
- hosts: servers
  roles:
    - { role: eniac111.mariadb }
```

## License

MIT / BSD

## Author Information

Created by [Blagovest Petrov](http://petrovs.info)
Based on the role of [Attila van der Velde](https://github.com/vdvm)
