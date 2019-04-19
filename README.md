# Ansible role : Ansible

![](https://img.shields.io/github/release/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/repo-size/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/release-date/Pandemonium1986/ansible-role-ansible.svg)
![](https://img.shields.io/github/license/Pandemonium1986/ansible-role-ansible.svg)

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
