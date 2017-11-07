# Ansible Role: OpenResty

[![Build Status](https://travis-ci.org/Lusitaniae/ansible-role-openresty.svg?branch=master)](https://travis-ci.org/Lusitaniae/ansible-role-openresty)

Installs OpenResty on RedHat/CentOS and Debian/Ubuntu servers.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    # Install OpenResty Package Manager and OpenResty Doc
    openresty_recommended_install: yes

    # Packages installed for yum systems.
    openresty_recommended_yum:
      - openresty-resty
      - openresty-opm
      - openresty-doc

    # Protocol to be used for package download.
    openresty_repo_protocol: https



## Dependencies

None.

## Example Playbook

    - hosts: openresty

      roles:
        - { role: Lusitaniae.openresty }


## License

MIT
