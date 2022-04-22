Install dependencies

```bash
ansible-galaxy install -r reuirements.yml
```

Common configuration:
```bash
ansible-playbook -i inventories/production/hosts --extra-vars "ansible_sudo_pass=<sudo_password>" --extra-vars "ansible_python_interperter=/usr/bin/python3" common.yml
```

Setup cluster:
```bash
ansible-playbook -i inventories/production/hosts --extra-vars "ansible_sudo_pass=<sudo_password>" --extra-vars "ansible_python_interperter=/usr/bin/python3" mariadb_cluster.yml
```

Setup HAProxy:
```bash
ansible-playbook -i inventories/production/hosts --extra-vars "ansible_sudo_pass=<sudo_password>" --extra-vars "ansible_python_interperter=/usr/bin/python3" haproxy.yml
```

Setup PHPMyAdmin:
```bash
ansible-playbook -i inventories/production/hosts --extra-vars "ansible_sudo_pass=<sudo_password>" --extra-vars "ansible_python_interperter=/usr/bin/python3" phpmyadmin.yml
```

