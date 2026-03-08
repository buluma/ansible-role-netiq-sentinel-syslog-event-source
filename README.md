# [Ansible role netiq-sentinel-syslog-event-source](#ansible-role-netiq-sentinel-syslog-event-source)

Ansible role for setting up a linux host as an event source to NetIQ Sentinel.

|GitHub|Issues|Pull Requests|Version|Downloads|
|------|------|-------------|-------|---------|
|[![github](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/actions/workflows/molecule.yml)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/pulls/)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-netiq-sentinel-syslog-event-source.svg)](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/releases/)|[![Ansible Role](https://img.shields.io/ansible/role/d/buluma/netiq-sentinel-syslog-event-source)](https://galaxy.ansible.com/ui/standalone/roles/buluma/netiq-sentinel-syslog-event-source/documentation)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- become: true
  gather_facts: true
  hosts: all
  name: Converge
  roles:
    - role: buluma.netiq_sentinel_syslog_event_source
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/molecule/default/prepare.yml):

```yaml
---
- become: true
  gather_facts: false
  hosts: all
  name: Prepare
  roles:
    - role: buluma.bootstrap
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/defaults/main.yml):

```yaml
---
sentinel_syslog_port: 1468
sentinel_syslog_protocol: tcp
sentinel_syslog_server: sentinel.example.com
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub |
|-------------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Build Status GitHub](https://github.com/buluma/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions)|

## [Context](#context)

This role is part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/robertdebock):

|container|tags|
|---------|----|
|[opensuse](https://hub.docker.com/r/robertdebock/opensuse)|all|
|[EL](https://hub.docker.com/r/robertdebock/enterpriselinux)|all|
|[Fedora](https://hub.docker.com/r/robertdebock/fedora)|all|

The minimum version of Ansible required is 2.4, tests have been done on:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them on [GitHub](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/issues).

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-netiq-sentinel-syslog-event-source/blob/master/LICENSE).

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
