Role Name
=========

An Ansible role to install the Onionperf in a given Virtual Environment.

Requirements
------------

This role has been tested with Ansible version 2.2.1.0

Role Variables
--------------

virtualenv_path must be defined, in order for pip to install Onionperf.

	repo: "https://github.com/robgjansen/onionperf.git" # Git repository
	git_tag: "master" # Git branch or tag to check out
	virtualenv_path: "" # Virtual Environment where Onionperf will be installed

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: parmegv.ansible-onionperf, virtualenv-path: "~/.virtualenvs/tor-browser-crawler" }

License
-------

BSD

Author Information
------------------

Rafael Gálvez Vizcaíno
Ph.D. student at ESAT/COSIC KU Leuven
