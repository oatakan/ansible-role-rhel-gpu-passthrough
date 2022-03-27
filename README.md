# ansible-role-rhel_gpu_passthrough
This repo contains an Ansible role enables GPU passthrough on a RHEL based system.

Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here.

> **_Note:_** This role is provided as an example only. Do not use this in production. You can fork/clone and add/remove steps for your environment based on your organization's security and operational requirements.

Requirements
------------

This role is only tested with NVIDIA GPUs but it should work with other devices including non GPU devices.

Role Variables
--------------

pci_device_key_name: NVIDIA # you can specify multiple matches here i.e. NVIDIA|AMD

Dependencies
------------

A list of roles that this role utilizes.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: enable gpu passthrough
      hosts: all
      gather_facts: False
      connection: local
      become: no
 
      roles:
        - oatakan.rhel_gpu_passthrough

License
-------

MIT

Author Information
------------------

Orcun Atakan