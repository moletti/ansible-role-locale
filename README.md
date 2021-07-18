Ansible role: Locale
=========

Base role for managing apt locales.

Install
------------
```
ansible-galaxy install moletti.locale
```

Example playbook
------------
```yaml
- hosts: all
  gather_facts: yes
  roles:
    - { role: moletti.locale, tags: locale }
```

Role Variables
--------------
|  variable    | type   | default     | description                                   |
|--------------|--------|-------------|-----------------------------------------------|
| locale       | str    | en_US.UTF-8 | Name and encoding of the locale               |
| locale_state | str    | present     | Whether the locale shall be present or absent |

LICENSE
-------
[MIT](/LICENSE)