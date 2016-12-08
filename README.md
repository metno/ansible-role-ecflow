ecflow
=========
This rols installs a ecflow server and/or client and/or python-library


Requirements
------------

None.

Role Variables
--------------
`daemon_user` - The user the server will run as
`deamon_home` - The home directory of the deamon
`deamon_port` - The port to listen to
`logserver_port` - The port the ecflow logserver will listen to
`genkeys_daemon_user` - Genrate ssh keys for the deamon user. Default = no
`systemd_env_vars` - systemd environment variables.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: apply configuration to ubuntu hosts
      hosts: ecflow
      remote_user: ubuntu
      become: yes
      become_method: sudo

License
-------

GNU GPLv2.

Author Information
------------------

Author: Espen Myrland <espenm@met.no>