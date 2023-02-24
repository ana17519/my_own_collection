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