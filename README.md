# Ansible-role-fluxbb

[FluxBB](https://fluxbb.org/) is designed as a lighter, faster alternative to some of the traditional feature heavy forum applications. It is easy to use and has a proven track record of stability and security making it an ideal choice of forum for your website.


## Roles varaiables

| Variable name | Default value | Description |
|---------------|-------|-------------|
| _postgresql_database | "fluxDB" | Create database |
| _postgresql_database_user | "fluxuser" | Username for the database |
| _postgresql_database_password | "fluxpassword" | Password for the database |


## Sample example of use in a playbook


The following code has been tested with Ubuntu 20.04

```yaml
- name: "Install FLuxBB"
  hosts: enter your hosts file
  become: yes
  roles:
    - ansible-role-fluxbb
  
  vars:
    _postgresql_database_user: ""
    _postgresql_database_password: ""
    _postgresql_database: ""
```

## Contributing

Don’t hesitate to create a pull request
