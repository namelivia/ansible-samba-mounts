# Samba mounts Ansible role [![Ansible Lint](https://github.com/namelivia/ansible-samba-mounts/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/namelivia/ansible-samba-mounts/actions/workflows/ansible-lint.yml)

The project depends on the collection `ansible.posix` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - ansible.posix

roles:
  - src: https://github.com/namelivia/ansible-samba-mounts
```

## Required variables
 - `samba_username` Username for the samba server.
 - `samba_password` Password for the samba server.
 - `samba_host_ip` IP address for the samba server.
 - `remote_folder` Remote folder to mount.
 - `local_folder` Local folder in wich will be mounted.
