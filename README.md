Ansible Role YUM Extra Packages for Enterprise Linux (EPEL)
=========

[![Build Status](https://travis-ci.org/Turgon37/ansible-yum-epel.svg?branch=master)](https://travis-ci.org/Turgon37/ansible-yum-epel)

:warning: This role is under development, some important (and possibly breaking) changes may happend. Don't use it in production level environments but you can eventually base your own role on this one :hammer:

:grey_exclamation: Before using this role, please know that all my Ansible roles are fully written and accustomed to my IT infrastructure. So, even if they are as generic as possible they will not necessarily fill your needs, I advice you to carrefully analyse what they do and evaluate their capability to be installed securely on your servers.

**This roles configure EPEL repositories on the hosts. This repository is required is some case to obtains some packages or packages versions**

## Features

Currently this role provide the following features :

  * EPEL repository configuration

## Requirements

### OS Family

This role is available for RedHat/CentOS

### Dependencies


## Role Variables

The variables that can be passed to this role and a brief description about them are as follows:

| Name              | Types/Values | Description                       |
| ------------------| -------------|---------------------------------- |
| yum_epel__enabled | Boolean      | Enable or not the EPEL repository |


## Example Playbook

To use this role create or update your playbook according the following example :


```
    - hosts: servers
      roles:
         - yum-epel
```


## License

MIT