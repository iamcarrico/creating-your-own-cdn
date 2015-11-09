## More config

```yml
- name: All Packages from apt-get
  apt: name={{ item }} state=installed
  with_items:
    - git
    - curl
    - htop
    - ntp
    - sendmail
    - mailutils
    - unzip
```

Note:
More configuration can happen task to task— this small example pulls in all the apt-get packages that we need on the server. All of these will be installed on any server that we designate.
