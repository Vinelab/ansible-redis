# Ansible Redis
Install and configure Redis on Centos/Red Hat with Ansible

## Installation
- Clone this repository inside your ```roles``` directory
or add as submodule: `git submodule add git@github.com:Vinelab/ansible-redis roles/redis`

- In your playbook:

```yaml
roles:
  - redis
```

## Synopsis
Redis will be installed as a service in ```/etc/init.d/redis```
allowing commands such as ```service redis start``` and ```service redis stop```
for easy management.

## Usage

```yaml
vars:

  redis: { version: 2.8.8 }
```
