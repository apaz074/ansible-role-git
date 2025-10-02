# Ansible Role: Git

An Ansible role to install and configure Git.

## Description

This role installs Git on various Linux distributions and allows for global configuration of the user name, email, and default branch name.

## Requirements

- Ansible 2.9 or higher.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

| Variable                  | Default Value         | Description                           |
| ------------------------- | --------------------- | ------------------------------------- |
| `git_user_name`           | `"John Doe"`          | The user name to configure globally.  |
| `git_user_email`          | `"johndoe@example.com"` | The user email to configure globally. |
| `git_default_branch_name` | `"main"`              | The default branch name for new repos.|

## Dependencies

None.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - role: ansible-role-git
      vars:
        git_user_name: "Your Name"
        git_user_email: "your.email@example.com"
        git_default_branch_name: "main"
```

## Supported Platforms

This role has been tested on the following platforms:

- Debian family (Debian, Ubuntu)
- RedHat family (CentOS, Fedora, RHEL)
- Archlinux family

## License

MIT

## Author Information

This role was created in 2025 by [your name].
