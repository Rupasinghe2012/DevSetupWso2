# Ansible Role: Jar

This role is used for adding the relavent jar files to product lib folder . 


Role Variables
--------------

There are no defaults variables in defaults/main.yml

Following variables are in the vars/main.yml
This variables are used to define the product home and the appuser:

```yaml
  EI_Home: /opt//EI/wso2ei-6.1.1
  API_Home: /opt/API
  app_user: mitra
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - Jar
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
