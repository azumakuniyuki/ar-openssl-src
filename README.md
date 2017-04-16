Ansible Role: openssl(src)
================================================================================
Build and install OpenSSL from a source code

- Build OpenSSL from a source code at /usr/local/src
- Install OpenSSL into /opt/openssl

Requirements
--------------------------------------------------------------------------------
None.

Role Variables
--------------------------------------------------------------------------------
The following variables are defined in defaults/main.yml file.

```yaml
openssl:
  rebuild: false
  version: "1.0.2k"
  install: "/opt/openssl"
  workingdir: "/usr/local/src"
```

Dependencies
--------------------------------------------------------------------------------
None.

Example Playbook
--------------------------------------------------------------------------------
```yaml
- hosts: all
  roles:
    - { role: azumakuniyuki.ar-openssl-src, openssl.version: "1.0.2p" }
```

License
--------------------------------------------------------------------------------
BSD

Author Information
--------------------------------------------------------------------------------
[azumakuniyuki](http://nyaan.jp/)

