WordPress Basic
===============

- Wordpress installation to get up and running with minimal fuss and complexity.
- The focus of the role is simplicity and sane defaults over unnecessary flexibility
- Documentation intended to be clear, complete and requiring minimal knowledge to get working.
- Installs PHP and NGINX on Ubuntu 16.04 (Not tested on other distributions)
- Bring your own database (Assuming mysql or mariadb)

Requirements
------------

- Pre-existing mysql or mariadb database with pre-existing user

Role Variables
--------------

- Keep your role variables under ansible/group_vars/<site-name>/wordpress.yml
- Example (Can be used as-is)

```
---

```

Dependencies
------------

- MySQL DB (Single node, Percona cluster or RDS if on AWS) Optional: geerlingguy.mysql (Or any other role that gets a basic mysql db up and running with minimal fuss)
- Ubuntu 16.04 Server

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
    - hosts: engeneon-web
      become: yes
      roles:
         - { role: archmangler.wordpress-basic, x: 42 }
```

License
-------

BSD

Author Information
------------------

Traiano G. Welcome (traiano@gmail.com)
