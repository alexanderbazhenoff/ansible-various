# ansible network role

This ansible role enables to configure various network components on remote linux distros.
Supports Centos 7, Ubunut 14/16.

- Ethernet Interfaces [+]
- Bridge Interfaces [+]
- Bonding interfaces [-]
- Routes in the machine [-]

Currently only ethernet and linux brdige network interfaces allowed.

**Usage**:
1. Specify hosts in inventory file
2. `ansible-playbook test_add_bridge.yml -i inventory`

or read *example.yml for details.

**Warning**: When you use the same params on the same hosts the role should be work ONCE (next run will broke the network settings).
