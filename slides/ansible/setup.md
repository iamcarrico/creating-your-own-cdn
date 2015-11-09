## Setup server

```YML
- name: "Create a first user"
  hosts: liger.iamcarrico.com
  remote_user: root
  tasks:
    - name: "Create a new user"
      user: name=ian shell=/bin/bash
    - name: "Create .ssh folder for the user"
      file: path=/home/ian/.ssh owner=ian group=ian state=directory mode=0775
    - name: "Pull down the ssh keys for the user"
      get_url: url=https://github.com/iamcarrico.keys dest=/home/ian/.ssh/authorized_keys mode=0600
```

`setup.yml`

Note:
This simple config file will do exactly what the name tags expect. It creates a new users, creates a `.ssh` file, then downloads my keys from GitHub to allow me to login. A more complete version of this script that I use for my production servers can be found at: https://github.com/iamcarrico/iamcarrico.server/blob/master/ansible/roles/setup/tasks/main.yml
