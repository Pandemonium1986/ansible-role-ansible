# Ansible role : Ansible

![Ansible Role](https://img.shields.io/ansible/role/37338?logo=ansible)
![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline/Pandemonium1986/ansible-role-ansible?logo=gitlab)
![GitHub release](https://img.shields.io/github/release/Pandemonium1986/ansible-role-ansible.svg?logo=github)
![Github license](https://img.shields.io/github/license/Pandemonium1986/ansible-role-ansible.svg?logo=github)
![Ansible Quality Score](https://img.shields.io/ansible/quality/37338?logo=ansible)

## DISCLAIMER

This role is no longer support. Please refer to the role [ansible-role-pip](https://github.com/Pandemonium1986/ansible-role-pip)

Install and configure ansible, ansible-lint and molecule.

## Requirements

This role is not self contained. He requires pandemonium1986.pip to work correctly.

```sh
  ansible-galaxy install -f pandemonium1986.pip
```

## Role Variables

From defaults/main.yml :

```yaml
ansible_users:
  - pandemonium
```

## Dependencies

None.

## Example Playbook

```yaml
- name :         Ansible play
  hosts :        pandama
  become:        true
  become_method: sudo
  become_user:   root
  tasks:
    - import_role:
        name:    pandemonium1986.ansible
```

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details

## Author Information

-   **Michael Maffait** - _Initial work_ - [Pandemonium1986](https://github.com/Pandemonium1986)
