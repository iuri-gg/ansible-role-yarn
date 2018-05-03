Ansible Role: YARN Repository
=========

[![Build Status](https://travis-ci.org/ocha/ansible-role-yarn.svg?branch=master)](https://travis-ci.org/ocha/ansible-role-yarn)
[![Ansible Galaxy](https://img.shields.io/ansible/role/13308.svg)](https://galaxy.ansible.com/ocha/yarn/)

Installs the [YARN Package Manager](https://yarnpkg.com) for Ubuntu/RHEL/CentOS.

Requirements
------------

This role only runs on Ubuntu, RHEL and its derivatives.
It requires EPEL repo on RHEL so it can install NodeJS.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    yarn_debian_repo_url: "https://dl.yarnpkg.com/debian/ stable main"
    yarn_debian_repo_gpg_key_url: "https://dl.yarnpkg.com/debian/pubkey.gpg"
    yarn_rhel_repo_url: "https://dl.yarnpkg.com/rpm/"
    yarn_rhel_repo_gpg_key_url: "https://dl.yarnpkg.com/rpm/pubkey.gpg"

Generally, these should not be changed, but if this role is out of date, or if you need a very specific version, these can be overridden.


Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - ocha.yarn

License
-------

MIT / BSD

Author Information
------------------

This role was created by [Iuri Gagnidze](https://www.github.com/ocha)
