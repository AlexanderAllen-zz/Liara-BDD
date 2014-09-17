Liara/BDD
=============

Ansible role for installing various Behavior Driven Development (BDD) related tools.

Requirements
------------

- PHP
- Composer, provided by `Liara.Composer`.

Role Variables
--------------

This role installs composer to `composer_path` and makes any binaries downloaded by Composer
to `composer_bin_dir` available to the environment through `/etc/environment`.

Required variables specified inside the `vars/main.yml` of `Liara.Composer`:

    # Path to user Composer directory.
    liara_composer_user_dir: /usr/local/bin/composer

Dependencies
------------

This role leverages `Liara.Composer` for installing Composer globally.

Example Playbook
----------------

    - hosts: webservers
      roles:
         - { role: AlexanderAllen.Liara-BDD }

License
-------

GPLv2

Author Information
------------------

https://github.com/AlexanderAllen
