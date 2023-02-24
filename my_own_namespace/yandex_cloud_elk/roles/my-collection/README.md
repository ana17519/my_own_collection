My collection
=========

This role will create file with content using custom module

Requirements
------------

Need to load custom module to .ansible/plugins/modules

Role Variables
--------------


| vars                  | description                              |
|-----------------------|------------------------------------------|
| path        | location to store file                   |
|state | deafault value is touch - to create file | 
|content | file content                             | 



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
- name: My own module
  hosts: localhost
  roles:
    - my-collection
```

License
-------

MIT

Author Information
------------------

Anastasiya Sukhodola