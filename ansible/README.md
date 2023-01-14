# Configuration provisionning
## Run playbook 

```
ansible-playbook -i inventories/hosts.yaml playbooks/admin.yaml -u user -b -e "ansible_sudo_pass=password"
```

