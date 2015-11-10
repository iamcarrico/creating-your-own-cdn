## Set up

* Access to repository
* Access to server
* Any other commands you want to run

Note:
Setting up DeployBot only has to happen once, but is a little bit of work. You have to give access to your GitHub (or other) repository. Give it access to your servers— that can happen with direct access to your server with an SSH key, or API access to many different services. Personally, I use access with an SSH key to my Digital Ocean servers.

You can also run commands before or after deployment on the box itself— for example, I use it to restart varnish (caching) on my box.
