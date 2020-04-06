# Running

```bash
ansible-playbook -i production.yml kubernetes.yml --vault-password-file .vault_password
```

## Setting up databases

Gitea needs:

create database gitea default character set utf8 default collate utf8_bin;
CREATE OR REPLACE USER gitea@'%' IDENTIFIED BY 'f132afsdf23asdf';
GRANT ALL PRIVILEGES ON gitea.* to gitea@'%' IDENTIFIED BY 'f132afsdf23asdf';