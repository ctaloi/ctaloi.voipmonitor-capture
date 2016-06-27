Role Name
=========

Install and configure a VoIP monitor capture node.
Tasks taken from [installation docs](http://www.voipmonitor.org/doc/Ubuntu_16.04_LTS)

Requirements
------------

Nothing specific

Role Variables
--------------

Defaults are defined in default/main.yml and can be overridden using role based variables when calling the role in your playbook as shown in the example playbook below

Dependencies
------------

None

Example Playbook
----------------

```
- name: Configure a new VoIP monitor capture server
  hosts:
    - voipmonitor-capture

    roles:
      - { role: voipmonitor-capture,
            voipmon_db_host: 192.168.1.2,
            voipmon_db_username: voipmonitor,
            voipmon_db_password: superSecret,
            voipmon_interface: eth0
          }
```

License
-------

BSD

Author Information
------------------

Chris Aloi
https://github.com/ctaloi
