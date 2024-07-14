# Ansible template project for home router.

This git repo is meant to be used as a starting point for setting up a Linux
system as a home router.

I like running home router inside LXC container, so the inventory is organized
as there's a Proxmox VE host and a router which is an LXC container.

As all the ansible roles and this start-kit project are started more than 2 years
ago, there must be something that's broken.

`site.yml` can be used to run all playbooks.


## How to override role config

In `group_vars` dir, create a file with the name of the role (which is also the
group name in the inventory). Copy role's `default/main.yml` to that file and
edit.

