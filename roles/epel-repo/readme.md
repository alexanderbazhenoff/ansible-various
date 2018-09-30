## Epel repository role role
Installs EPEL repository for RedHat family distros.

**Required**: ansbible>=1.9.4.

**Usage:** Use global hosts settings (readme will be updated) or run *example.yml files to override them:
1. Specify hosts in **epel-repo/inventory** file.
2. Run: `test install_epel_example.yml -i inventory` or `ansible-playbook test.yml -i inventory --aks-pass` if you don't want to set password in plain text file.
