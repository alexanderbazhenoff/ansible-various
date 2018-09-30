## Linux Kernel Virtual Machine ansible role
Installs KVM for Centos 7.x and Ubuntu 14/16 distros.

**Required**: ansbible>=1.9.4.

**Usage:** Use global hosts settings (readme will be updated) or run *example.yml files to override them:
1. Specify hosts in **epel-repo/inventory** file.
2. Run: `ansible-playbook test.yml -i inventory` or `ansible-playbook test.yml -i inventory --aks-pass` if you don't want to set password in plain text file.

Uncluding this role example:

`- hosts: all
  become: true
  become_method: sudo
  roles:
    - role: kvm`

or:

`- hosts: all
  become: true
  become_method: sudo
  roles:
    - { role: kvm, kvm_delete_default_networok: false }`

if you don't want to remove default KVM network (wich was created after KVM install).

Check `defaults/main.yml` for ***other variables***.
