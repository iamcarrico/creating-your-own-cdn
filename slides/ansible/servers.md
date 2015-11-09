## More servers

```yml
[production]
newyork.iamcarrico.com
amsterdam.iamcarrico.com
singapore.iamcarrico.com
sanfrancisco.iamcarrico.com

[staging]
liger.iamcarrico.com
```

```bash
ansible-playbook -i hosts playbook.yml --limit production
```

Note:
This will allow me to run all the configuration I have setup on ALL of my production servers at the same time. Anything in `playbook.yml` will be ran concurrently, ensuring new servers are setup appropriately and any existing servers are updated.
