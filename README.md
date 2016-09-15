ansible-role-sts 
=========

An ansible role that installs an configures an Spring Source Tool Suite IDE in Ubuntu

It will download STS, and create the needed menu links.

Requirements
------------

- Java JDK 8+ 

Variables
---------

- __sts_version__: number version of product. By default: _3.8.1.RELEASE_
- __sts_url__: official download url from [http://spring.io]()
- __sts_download_dir__: _/tmp_  by default
- __sts_install_dir__: By default STS will be installed in _/opt_
- __sts_file_dist__: the complete final name of artifact: `spring-tool-suite-{{ sts_version }}.tar.gz`

Dependencies
------------
JDK8 [mrlesmithjr.oracle-java8](https://galaxy.ansible.com/mrlesmithjr/oracle-java8/)

Example Playbook
----------------

You can use it like:

```yml
- hosts: local
  roles:
    - dpalomar.sts
```

Install in your computer
------------------------

If you just want to run this in your machine, you can:

```console
$ git clone https://github.com/dpalomar/ansible-role-sts
$ cd ansible-role-sts
$ ansible-galaxy install -r requirements.yml
```

- You'll need Ansible 2.2+ installed;
- Running this will also install JDK 8.

License
-------

MIT / BSD


