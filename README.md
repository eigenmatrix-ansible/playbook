# Eigenmatrix Ansible Deployment

With this playbook, you can run your own matrix homeserver including many bridges and extra features such as HTTP routing for all your traffic. The playbook is intended to be cloned and then only needs to be configured for your hosts by editing `host_vars/`. Multiple deplyments to the same physical server are supported by allowing to have everything namespaced.

## Usage

```
git clone https://github.com/eigenmatrix-ansible/playbook.git
vim host_vars/matrix.myserver.tld # Editing your host
ansible-playbook site.yml
```

## Project scope

- [ ] Synapse with worker support (using postgres+redis)
- [ ] Support many bridges to popular platforms
- [ ] Ability for namespacing everything to allow multiple deployments to the same server
... more to be added

