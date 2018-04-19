# Ansible Role: EISetup

This role is used for Downloading the Fresh Enterprise Integrator to the Server.


Role Variables
--------------
In the Default variables there is a variable to clean install the EI product. Initialy it's true. After initial creation you can change it to false.
```yaml
    clean_install: true 
```

Bellow variable are common variables that related to the product installations. 

```yaml
    app_user: mitra
    key_pub: id_rsa.pub
    key_piv: id_rsa
    doc_root: /opt//EI/wso2ei-6.1.1
```

Following Variables are related WsO2 product related tuning parameters.
```yaml
    Xms_Value: 2048
    Xmx_Value: 4096
    wk_pool_size_core: 1600
    wk_pool_size_max: 2000
    max_host: 2000
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - EISetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
