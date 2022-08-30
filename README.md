# Ansible-role-mybb

[MyBB](https://mybb.com/) is the free and open source forum software powering thousands of engaging, vibrant, and unique communities across the internet.


## Roles varaiables

| Variable name | Default value | Description |
|---------------|-------|-------------|
| _postgresql_database | "mybb" | Create database |
| _postgresql_database_user | "admin" | Username for the database |
| _postgresql_database_password | "admin" | Password for the database |


## Sample example of use in a playbook


The following code has been tested with Ubuntu 20.04

```yaml
- name: "install mybb"
  hosts: enter your hosts file
  become: yes
  roles:
    - ansible-role-mybb
  
  vars:
    _postgresql_database_user: ""
    _postgresql_database_password: ""
    _postgresql_database: ""
```

## Contributing

Don’t hesitate to create a pull request

