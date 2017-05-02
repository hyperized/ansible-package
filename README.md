hyperized.package
=========

Simple Ubuntu APT package wrapper

Requirements
------------

Ansible 2.1 or above is highly recommended.

Role Variables
--------------

	package_state: installed
	package_name: yourpackage
	package_cache_valid_time: 3600 (overridden by apt_cache_valid_time)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - { role: hyperized.package, package_name: htop }

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben.geijteman@fdmediagroep.nl>
