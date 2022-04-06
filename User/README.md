
# Ansible Create User

0. Create file vars with public key and encrypte
```console
nano secret_key.yml
---
public_key_content: |
  ssh-rsa AAAAB3Nza...gyGwGE= user1@system

ansible-vault encrypt secret_key.yml
```

1. Play with ask vault pass
```console
ansible-playbook playbook-create-user.yml --ask-vault-pass
```

2. Ckeck user list and remove user1
```console
sudo less /etc/passwd
sudo deluser user1
```