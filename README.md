# Remote desktop Ansible role

Installs a XFCE4 desktop + XRDP on Ubuntu so windows, mac or linux users can log in.

## Requirements

Requires a ssh tunnel to work - password login is restricted to localhost.

Also requires creating passwords in an acceptable format for Ansible.

## Role variables

    ubuntu_password: '$1$salty$NydFn6/MeEY/Dc0QmWWah1'
    
The decrypted default password is 'hello there'.

## Example Playbook

    - hosts: all
      roles:
        - remote-desktop
