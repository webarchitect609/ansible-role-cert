Ansible Role: Cert
==================

[![Build Status](https://github.com/webarchitect609/ansible-role-cert/actions/workflows/build.yml/badge.svg)](https://github.com/webarchitect609/ansible-role-cert/actions/workflows/build.yml)
[![Latest version](https://img.shields.io/github/v/tag/webarchitect609/ansible-role-cert?sort=semver)](https://github.com/webarchitect609/ansible-role-cert/releases)

[![Downloads](https://img.shields.io/ansible/role/d/webarchitect609/cert)](https://galaxy.ansible.com/ui/standalone/roles/webarchitect609/cert)
[![License](https://img.shields.io/github/license/webarchitect609/ansible-role-cert)](LICENSE.md)
[![More stuff from me](https://img.shields.io/badge/galaxy-webarchitect609-000)](https://galaxy.ansible.com/ui/standalone/namespaces/7493/)

Installs ca-certs for ssl from the list of URLs.

Requirements
------------

None.

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: webarchitect609.cert }
  vars:
    cert_urls:
      - "https://gu-st.ru/content/lending/russian_trusted_root_ca_pem.crt"
      - "https://gu-st.ru/content/lending/russian_trusted_sub_ca_pem.crt"

```

License & Author Information
----------------------------

[BSD-3-Clause](LICENSE.md)
