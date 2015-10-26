# Ansible Role: adeya-vmware-tools

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):
vmwaretools_tools_version: latest
* vmwaretools_yum_server: http://packages.vmware.com
* vmwaretools_key_name: /tools/keys/VMWARE-PACKAGING-GPG-RSA-KEY.pub
* vmwaretools_repo_enabled: 1
* vmwaretools_esxi_version: 5.5p02
* vmwaretools_pkgs:
  * vmware-tools-esx-kmods
  * vmware-tools-esx-nox
  * vmware-tools-vmxnet3-common
  * vmware-tools-pvscsi-common
  * vmware-tools-vmmemctl-common
* vmwaretools_uninstall_dir: /root/vmware-tools-distrib
* vmwaretools_uninstall_file: /root/vmware-tools-distrib/bin/vmware-uninstall-tools.pl
* vmtools_reboot_confirmation: false

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
         - adeya-vmware-tools

## License

GPLv2

## Author Information

This role was created in 2015 by **Oussama Hammami @ adeya SA**
