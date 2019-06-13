Ansible role: LXD
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-lxd.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-lxd)

Establish and configure LXD/LXC for Linux using either a native or a snap package.

Requirements
------------

None

Role Variables
--------------

Optional arguments:

    configuration: <dict, preseed configuration in YAML format>
    profiles: <list, individual profiles in YAML format>
    use_snap: <bool, use snap package instead of native package>

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: lxd
          vars:
            use_snap: no
            configuration: {}

License
-------

MIT

Author Information
------------------

Tibor Csóka
