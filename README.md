# ansible-role-shell
Role for shell setup


## Usage

in requirements.yml:
```yml
- src: git+ssh://git@github.com/your_username/your_repo.git
  scm: git
  version: branch_or_tag_name

```

Then `ansible-galaxy install -r requirements.yml -p ./roles`

In the playbook.yml:

```yml
---
- hosts: your_hosts
  roles:
    - role: role_name
      vars:
        variable_name: value

```