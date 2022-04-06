
# Ansible Install and Remove postfix

1. Install
```console
sudo ansible-playbook playbook-postfix.yml --tags init 
```

1. Remove
```console
sudo ansible-playbook playbook-postfix.yml --tags drop 
```
