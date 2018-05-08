1. Install required Ansible roles
```
ansible-galaxy -r requiremetns.yml
```

2. Create nodes VMs
```
vagrant up
```

3. Run Ansible playbook
```
ansible-playbook -i staging fairnet.yml
```
