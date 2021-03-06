# Instack ManageIQ Pull Request Testing Helper Scripts

## Prerequisities

 * virt-builder from libguestfs-tools package
 * deployed undercloud with instack VM running

## Usage

To create VM with ManageIQ source code from custom user and branch use:

```sh
./miq_deploy_from -u Ladas -b openstack_infra_ui_for_openstack_components -i miq.qcow2
```

This will prepare `miq.qcow2` image, checkout ManageIQ source code from `https://github.com/Ladas/manageiq.git` using `openstack_infra_ui_for_openstack_components` branch.
After first boot VM will have ManageIQ running and script will register Instack Undercloud as OpenStack Infra Provider in ManageIQ.
