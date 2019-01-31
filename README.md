# Ansible role : Ansible

![](https://img.shields.io/github/release/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/repo-size/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/release-date/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/license/Pandemonium1986/ansible-role-ansible.svg)

Install and configure ansible, ansible-lint and molecule.

## Requirements

This roles is self contained and install pip from debian backports if needed.

## Role Variables

From vars/main.yml :

```yaml
apt_packages:
  - python-pip
  - python-dev
```

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: pandemonium1986.ansible }
```

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details

## Author Information

-   **Michael Maffait** - _Initial work_ - [Pandemonium1986](https://github.com/Pandemonium1986)
