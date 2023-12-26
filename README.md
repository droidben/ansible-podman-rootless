Role Name
=========

This ansible role is to install podman and enable rootless mode for the specified user.

Requirements
------------

This role requires ansible-core >= 2.12, as well as the following ansible collections:

* `ansible.posix`
* `containers.podman`

Role Variables
--------------

The roles variables are specified in the defaults dir. See below for an overview of avaibale variables:

```yaml
container_run_as_user: rootless_user
container_run_as_group: rootless_user
install_prerequisites: true
skip_preparation: false
systemd_scope: system
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - ansible-podman-rootless

License
-------

BSD

