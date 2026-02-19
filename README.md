**DEPRECATED: This role is no longer maintained. Please use [nvm's install script](https://github.com/nvm-sh/nvm#installing-and-updating) directly instead.**

---

Ansible Role: nvm
=========

Install NVM for the user running Ansible. It's expected NVM is loaded into your shell profile independently of this role.

Requirements
------------

The only prerequisite for this role is `git` is installed.

Role Variables
--------------

|Variable|Default|Description|
|--------|-------|-----------|
|`nvm_install_directory`|`~/.nvm`|Installation directory for NVM|
|`nvm_version`|`v0.34.0`|Version of NVM to lock the install to.|

Dependencies
------------

_None_

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - brianhartsock.nvm
         - role: brianhartsock.nvm
           become: yes
           become_user: mary


License
-------

MIT

Author Information
------------------

Created with love by [Brian Hartsock](http://blog.brianhartsock.com).
