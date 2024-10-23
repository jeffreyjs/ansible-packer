# Ansible Role: Packer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Install [Packer](https://www.packer.io) with ansible.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

Pin the version of packer to install, if omitted then it will query GitHub for the latest version. By default this is commented out.

```yaml
# packer_version: "1.0.0"
```

The state of packer on the machine, set to `install` or `remove`:

```yaml
packer_state: install
```

## Dependencies

None.

## Example Playbook

```yaml
- hosts: server
  roles:
    - jeffreyjs.packer
```

## License

MIT / BSD

## Author Information

[Jeffrey Swindel](https://github.com/jeffreyjs)
