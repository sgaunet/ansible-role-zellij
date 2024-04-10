# Ansible Role: zellij

[![CI](https://github.com/sgaunet/ansible-role-zellij/workflows/CI/badge.svg?event=push)](https://github.com/sgaunet/ansible-role-zellij/actions?query=workflow%3ACI)

An Ansible Role that installs [zellij][https://github.com/zellij-org/zellij] on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    zellij_version: "0.39.2"
    zellij_bin_path: "/usr/local/bin"
    zellij_tmp_directory: "{{ lookup('env', 'TMPDIR') | default('/tmp', true) }}"
    zellij_os: "unknown-linux-musl"
    zellij_arch: "x86_64"

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - sgaunet.zellij
```

## License

MIT
