LXD
=========

Establish and setup LXD.

Requirements
------------

None

Role Variables
--------------

    configuration: <the entire yaml preseed configuration>
    profiles: <list, profile list>
    use_snap: <yes if snap package should be used instead of package>

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

Tibor Csoka
