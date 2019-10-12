Ansible role: LXD
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-lxd.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-lxd)

Establish and configure LXC/LXD for Linux using either a native distribution package or a snap package.

Requirements
------------

None

Role Variables
--------------

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    lxd_use_snap_daemon: true

    lxd_profiles: []    # list of profiles to be loaded directly as YAML

    lxd_remotes: []     # list of remotes to be added

These variables can be specified:

    lxd_configuration: <dict, preseed configuration in YAML format>

`lxd_remote` content:

    lxd_remotes:
      - name:           # string
        url:            # string
        protocol:       # lxd|simplestreams

Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: lxd
          vars:
            lxd_use_snap_daemon: false

License
-------

MIT

Author Information
------------------

Tibor Csóka
