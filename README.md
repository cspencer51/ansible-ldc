ansible-ldc
=========

This role installs the DMD compiler (https://github.com/ldc-developers/ldc).


Role Variables
--------------

Variables to deploy role are listed below.

- ldc_install_dir
- ldc_version
- ldc_old_compilers

DMD install variables can be specified as follows:

```yml
ldc_install_dir: /usr/local
ldc_version: 1.29.0
ldc_old_compilers: [1.28.1]
```

Example Playbook
----------------

```yml
- name: Install ldc
  hosts: all
  roles:
    - name: Install ldc
      role: cspencer51.ldc
  tags:
    - ldc
  vars:
    ldc_install_dir: /usr/local
    ldc_version: 1.29.0
    ldc_old_compilers: [1.28.1]
```

License
-------

MIT
