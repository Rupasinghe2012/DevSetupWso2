# Ansible Role: API_AllInOne_Config

This role is used for setting up Cluster configurtaions and Certifactes adding to the AllInOne ApiManger product.

Requirments
--------------
Before you run this role you must run APISetup Role first.

Role Variables
--------------

For this role there are few variables used:

You can define the Api Manger cluster related domains
```yaml
  domain: am.mitra.com  
  mgt_gw_domain: mgt.gw.mitra.com
  gw_domain: gw.mitra.com
  km_domain: km.mitra.com
```

These Variables are for db credentails
```yaml
  db_user: apiadmin
  db_pass: apiadmin
```

Following variables are related to application
```yaml
  doc_root: /opt/API_APIManager/wso2am-2.1.0
  app_user: mitra
  local_port: 4300
  offset: 0
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
        - APISetup
        - API_AllInOne_ClusterSetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
