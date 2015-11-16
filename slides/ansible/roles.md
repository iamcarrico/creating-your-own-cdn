## Roles

```
- name: "Server setup tasks"
  hosts: all
  sudo: yes
  roles:
   - Ansibles.nginx
   - varnish
   - php
```

```
playbook.yml
```

Note:
Instead of storing all of your configuration in a single file, you can separate them into roles. This makes it much easier to organize parts of your configuration into specific... roles. Within a role, you can put configuration files, templates, or other important information. You can even organize some roles to run on some servers, and not on others.
