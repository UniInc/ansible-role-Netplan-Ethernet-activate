Netplan ethernet interface
=========

Configure Network Interfaces using Netplan!
Ideal for server OS'es.

Function:
- activate any inactive interface, with: dhcp

## Single Default Gateway
By default: added interface will use `use-routes: false` to prevent Duplicate Gateways breaking Internet access.
```
dhcp4-overrides:
    use-routes: false
```

you can confirm this with: `ip route`


https://unix.stackexchange.com/questions/517995/prevent-netplan-from-creating-default-routes-to-0-0-0-0-0

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
