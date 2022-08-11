# Ansible-exoscale-mybb

[MyBB](https://mybb.com/) is the free and open source forum software powering thousands of engaging, vibrant, and unique communities across the internet.


## Roles varaiables

| Variable name | Default value | Description |
|---------------|-------|-------------|
| postgresql_database | "mybb" | Create database |
| postgresql_database_user | "admin" | Username for the database |
| postgresql_database_password | "admin" | Password for the database |


## Sample example of use in a playbook


The following code has been tested with Ubuntu 20.04

```
- name: "install mybb"
  hosts: webserver
  become: yes
  roles:
    - ansible-exoscale-mybb
  
  vars:
    postgresql_database_user: ""
    postgresql_database_password: ""
    postgresql_database: ""
```

## Contributing

Don’t hesitate to create a pull request

