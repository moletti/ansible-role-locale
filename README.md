Ansible role: Locale
=========
[![Ansible Role](https://img.shields.io/ansible/role/55682)](https://galaxy.ansible.com/moletti/locale) [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/moletti/ansible-role-locale)](https://github.com/moletti/ansible-role-locale/releases) [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/moletti/ansible-role-locale/Ansible%20Molecule?label=test)](https://github.com/moletti/ansible-role-locale/actions/workflows/molecule.yml) [![Ansible Quality Score](https://img.shields.io/ansible/quality/55682)](https://galaxy.ansible.com/moletti/locale) [![Ansible Role](https://img.shields.io/ansible/role/d/55682)](https://galaxy.ansible.com/moletti/locale)

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
  vars:
    locale: "en_US.UTF-8"
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