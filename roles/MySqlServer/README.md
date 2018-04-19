# Ansible Role: MySQLServer

This role is used for creation for Enerprise Intergrator and API Mangager MySql DB setup from the scratch. This role can be used in Ubuntu, RedHat7 and AmazonLinux


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

  table_creation: true

This variable must set to true if you want to create relavent tables for you Databases.
There are os related variables also vars/Debian.yml vars/RedHat-6.yml vars/RedHat-7.yml

Following variables are in the vars/main.yml
This variable is for reading the sql queries in the product home:

```yaml
  EI_Home: /opt//EI/wso2ei-6.1.1
  API_Home: /opt/API/wso2am-2.1.0
```

Credentials for the Mysql:
```yaml
  mysql_root_pass: ""
  mysql_root_username: root
  mysql_users_pass: regadmin
  mysql_users:
    - regadmin
```
You can define the databases for relavent to the product
```yaml  
  mysql_databases:
  - WSO2_USER_DB
  - REGISTRY_DB
  - EI_ANALYTICS_EVENT_STORE_DB
  - EI_ANALYTICS_PROCESSED_DATA_STORE_DB
  - apimgtdb
  - statdb
  - API_ANALYTICS_EVENT_STORE_DB
  - API_ANALYTICS_PROCESSED_DATA_STORE_DB

```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - { role: MySqlServer, table_creation: false }
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
