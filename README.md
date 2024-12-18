# jdam-ansible-playbooks
An assortment of Ansible playbooks for the homelab community. Streamline your infrastructure automation with these shared configurations and setups, tailored for self-hosters and enthusiasts alike.

## Running the Playbooks

To run the playbooks, use the following command as en example when you are in the root directory of this project:

```bash
ansible-playbook -i inventory/proxmox.yaml -i inventory/static_hosts.yaml proxmox-playbooks/deployLXC.yaml --ask-pass
```
You will need to enter the ssh password since ansible will need to know what password to use when connecting to the LXC. after this playbook runs you can use the ansible user configured for any other playbooks with ssh.