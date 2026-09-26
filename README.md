# Infrastructure setup

Replace `test` with `production` to select the other environment. Ansible prompts for the vault password.

```bash
ansible-playbook playbooks/deploy.yml -i inventories/common -i inventories/test --ask-vault-pass
ansible-playbook playbooks/check.yml -i inventories/common -i inventories/test --ask-vault-pass
```