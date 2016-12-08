ecflow
=========
This role installs a ecflow server and/or client and/or python-library

Requirements
------------

None.

Role Variables
--------------
daemon_user: The user the server will run as
deamon_home: The home directory of the deamon
deamon_port: The port to listen to
logserver_port: The port the ecflow logserver will listen to
genkeys_daemon_user: Generate ssh keys for the deamon user. Default = no
systemd_env_vars: systemd environment variables.

Dependencies
------------

None.

Example Playbook
----------------

    - name: apply configuration to ubuntu hosts
      hosts: ecflow
      remote_user: ubuntu
      become: yes
      become_method: sudo
      roles:
        - ecflow
        - met-ecflow-support
License
-------

GNU GPLv2.

Author Information
------------------

Author: Espen Myrland <espenm@met.no>
