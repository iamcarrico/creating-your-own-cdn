## Roles

```
|-playbook.yml
|-roles
 |---php
 |-----handlers
 |-----tasks
  |-----main.yml
 |-----templates
 |---varnish
 |-----handlers
 |-----tasks
 |-----templates
```

Note:
If your playbook is in a base directory, then there must be a folder called `roles` with all the folders with the same names that you used in `playbook.yml`. Each folder has some sub-folders— the most important of which is tasks. Within tasks there is a `main.yml` that looks pretty much like the other playbook we looked at earlier. It will contain all of your tasks for that role.
