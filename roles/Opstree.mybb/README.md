Role Name
=========

This role installs mybb forum .


Dependencies
------------ 

it will install nginx php-fpm.

------------
Role Variables
--------------
Here we can provide parameters for varibles

- default/main.yml


***********parameters************

mybb_version: "1806"
nginx_root_path: "/var/www/html"
server_name: "mybb.com"
epel_repo_url: "https://dl.fedoraproject.org/pub/epel/epel-release-latest-{{ ansible_distribution_major_version }}.noarch.rpm"
epel_repo_gpg_key_url: "/etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}"



Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: mybb_hosts
      roles:
         - { role: Opstree.mybb }

License
-------

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
