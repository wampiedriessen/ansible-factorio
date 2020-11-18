Factorio
=========

This Ansible role installs and runs a factorio server, optionally for a given save file

Requirements
------------

A target machine with screen and systemd

Role Variables
--------------

If ran as-is, this role creates a Factorio server and starts a randomly generated map with default settings.
If you wish to continue on a previous save, supply the `factorio_save_file` variable with an absolute path to the save you would like to upload.
If you wish to alter the IP the server binds to, use `factorio_bind_ip`

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: wampie.factorio
          factorio_save_file: files/my_save_file.zip
          factorio_bind_ip: 10.18.0.8

License
-------

BSD

