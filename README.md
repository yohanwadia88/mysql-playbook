

Role to install and configure MySQL Database on RedHat and Debian based systems.
This role has been tested on the following OSs:
--CentOS 6.5
--Ubuntu 12.04

Requirements
------------

None

Role Variables
--------------

OS specific variables are defined in /vars/{{ ansible_os_family }}.yml files.
Default variables are defined in /defaults/main.yml
On execution, the playbook will prompt the user to enter the MySQL root password.

Dependencies
------------

None

Example Playbook
----------------

     - hosts: all
       vars_prompt:
        - name: "MySQLPass"
          prompt: "Enter MySQL root password"
          private: yes
          default: "P@$$w0rd"

       roles:
        - mysql




License
-------

BSD

Author Information
------------------

This role was authored by Yohan | 2015.


