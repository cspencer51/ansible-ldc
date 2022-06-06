ansible-dmd
=========

This role installs the DMD compiler (https://dlang.org/download.html).


Role Variables
--------------

Variables to deploy role are listed below.

- dmd_install_dir
- dmd_version

DMD install variables can be specified as follows:

```yml
dmd_install_dir: /usr/local/dmd
dmd_version: 2.098.1
old_compilers: [2.098.0]
```

Example Playbook
----------------

```yml
- name: Install dmd
  hosts: all
  roles:
    - name: Install dmd
      role: cspencer51.dmd
  tags:
    - dmd
  vars:
    dmd_install_dir: /usr/local/dmd
    dmd_version: 2.098.1
    old_compilers: [2.098.0]
```

License
-------

MIT
