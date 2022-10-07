👯 cisco\_nxos\_vpc
===================

🪄 Configure a pair of Cisco Nexus devices in virtual Port Channel (vPC).

Requirements
------------

💿 [Cisco NXOS Collection](https://galaxy.ansible.com/cisco/nxos)

Role Variables
--------------

vars/defaults.yml:
- vpc\_domain
- vpc\_peer\_portchannel\_id
- vpc\_peer\_portchannel\_if\_member\_1
- vpc\_peer\_portchannel\_if\_member\_2
- vpc\_keepalive\_if
- vpc\_keepalive\_vrf

hostvars:
- vpc\_keepalive\_ip
- vpc\_keepalive\_ip\_peer

Dependencies
------------

None.

Example Playbook
----------------

    ---
    - name: Configure a pair of Cisco Nexus devices in vPC.
      hosts: "{{ target }}"
      gather_facts: false

      roles:
        - role: cisco_nxos_vpc
          tags: vpc

License
-------

BSD

Author Information
------------------

Jørn Ivar Holland
