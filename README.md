Role Name
=========

Ansible Galaxy role for installing VSFTP

Role Variables
--------------

User accounts can be specified inside `vars/main.yml``
    
    vsftp:
      accounts: 
        - username: user1
          password: password1
          folder: /tmp/
        - username: user2
          password: password2
          folder: /var/www/

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: sparkfabrik.vsftp, vsftp_port: 21 }

License
-------

BSD
