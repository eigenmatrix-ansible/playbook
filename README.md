# Eigenmatrix Ansible Deployment

With this playbook, you can run your own matrix homeserver including many bridges and extra features such as HTTP routing for all your traffic. The playbook is intended to be cloned and then only needs to be configured for your hosts by editing `host_vars/`. Multiple deplyments to the same physical server are supported by allowing to have everything namespaced.

## Usage

```
git clone --recursive https://github.com/eigenmatrix-ansible/playbook.git
vim inventories/matrix/host_vars/matrix.myserver.tld # Editing your host
vim inventories/matrix/hosts.yml # add your host to the inventory
ansible-playbook ansible_collections/eigenmatrix/glue/playbooks/site.yml # until ansible 2.11 is released
```

## Project scope

- [ ] Synapse with worker support (using postgres+redis)
- [ ] Support many bridges to popular platforms
- [ ] Ability for namespacing everything to allow multiple deployments to the same server
... more to be added

