Bacn
=========

This role installs a Bacn web server

Requirements
------------

None

Role Variables
--------------

* domain_name: The domain name used to access the Bacn installation
* superuser: A username for the superuser account
* superuser_email: An email address for the superuser account
* superuser_password: A password for the superuser account
  
Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars_prompt:
        - name: domain_name
          prompt: Enter the domain name this installation of Bacn will be running on
          private: no
        - name: superuser
          prompt: Enter a username for Bacn superuser
          private: no
        - name: superuser_email
          prompt: Enter an email for Bacn superuser
          private: no
        - name: superuser_password
          prompt: Enter a password for Bacn superuser
          confirm: yes
          private: yes
      roles:
        - bacn

License
-------

BSD

Author Information
------------------

This was created by [Malcolm VanOrder](https://github.com/mvanorder)
