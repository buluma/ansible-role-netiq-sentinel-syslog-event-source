# [netiq-sentinel-syslog-event-source](#netiq-sentinel-syslog-event-source)

Ansible role for setting up a linux host as an event source to NetIQ Sentinel.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-netiq-sentinel-syslog-event-source)|[![quality](https://img.shields.io/ansible/quality/)](https://galaxy.ansible.com/buluma/netiq-sentinel-syslog-event-source)|[![downloads](https://img.shields.io/ansible/role/d/)](https://galaxy.ansible.com/buluma/netiq-sentinel-syslog-event-source)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.netiq_sentinel_syslog_event_source
```

The machine needs to be prepared. In CI this is done using `molecule/default/prepare.yml`:
```yaml
---
- name: prepare
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: buluma.bootstrap
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for netiq-sentinel-syslog-event-source
sentinel_syslog_server: sentinel.example.com
sentinel_syslog_port: 1468
sentinel_syslog_protocol: tcp
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/main/requirements.txt).

## [Status of used roles](#status-of-requirements)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | GitLab |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|[![Build Status GitLab ](https://gitlab.com/buluma/ansible-role-bootstrap/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-bootstrap)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|opensuse|all|
|el|all|
|fedora|all|

The minimum version of Ansible required is 2.4, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/CHANGELOG.md)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
