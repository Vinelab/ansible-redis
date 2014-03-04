# Ansible Redis
Install and configure Redis on Centos/Red Hat with Ansible

## Installation
Clone this repository inside your ```roles``` directory.

## Synopsis
Redis will be installed as a service in ```/etc/init.d/redis``` allowing commands such as ```service redis start``` and ```service redis stop``` for easy management.

## Usage
There must be an ```app``` var with ```redis``` inside it specifying the desired version to install as follows:

```
vars:

  app:
    redis:
      version: 2.8.6
````

> you may also specify ```app:``` in a separate YAML file and include it in ```vars_files```