# Ansible Role: APISetup

This role is used for Downloading the Fresh Enterprise Integrator to the Server and setting up product envoironment. This role include the Prduct tuning conf and parameters also.


Role Variables
--------------

For this role there is one variable used for definig the App User.

```yaml
    app_user: mitra
    key_pub: id_rsa.pub
    key_piv: id_rsa
    domain: mitra.com
    XMS: 4096
    XMX: 4096
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - APISetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
