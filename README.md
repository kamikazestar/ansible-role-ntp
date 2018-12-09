# Ansible role: NTP

/* [![Build Status](https://travis-ci.org/kamikazestar/ansible-role-os-upgrade.svg?branch=master)](https://travis-ci.org/kamikazestar/ansible-role-os-upgrade) */

This role will install, configure and run NTP

# Requirements

Currently this role don't require other role or libralies.

# Role Variables

Role is using variables listed below:

  - ntp_enabled - set to true by default
  - ntp_timezone - set to Etc/UTC by default
  - ntp_area - empty by default
  - ntp_servers
  - ntp_restrict - set to localhost by default

# Dependencies

This role currently don't have any dependencies itself, but for automated tests it's using [Jeff Geerling](https://hub.docker.com/u/geerlingguy/) Docker containers:

  - [docker-centos7-ansible](https://hub.docker.com/r/geerlingguy/docker-centos7-ansible/)
  - [docker-centos6-ansible](https://hub.docker.com/r/geerlingguy/docker-centos6-ansible/)
  - [docker-fedora29-ansible](https://hub.docker.com/r/geerlingguy/docker-fedora29-ansible/)
  - [docker-fedora27-ansible](https://hub.docker.com/r/geerlingguy/docker-fedora27-ansible/)
  - [docker-amazonlinux2-ansible](https://hub.docker.com/r/geerlingguy/docker-amazonlinux2-ansible/)
  - [docker-ubuntu1804-ansible](https://hub.docker.com/r/geerlingguy/docker-ubuntu1804-ansible/)
  - [docker-ubuntu1604-ansible](https://hub.docker.com/r/geerlingguy/docker-ubuntu1604-ansible/)
  - [docker-debian9-ansible](https://hub.docker.com/r/geerlingguy/docker-debian9-ansible/)
  - [docker-debian8-ansible](https://hub.docker.com/r/geerlingguy/docker-debian8-ansible/)


# Example Playbook

You can run this role as in example playbook below:

    - hosts: servers
      roles:
         - role: kamikazstar.ansible_role_ntp

# License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/kamikazestar/VagrantLab/blob/master/LICENSE) for details.

# Author Information

* **Marcin Slabonski** - *Initial work* - [kamikazestar](https://github.com/kamikazestar)
