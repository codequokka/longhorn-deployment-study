```
vscode@8efc42c9ad45:/workspace/ansible$ ansible-galaxy install -r requirements.yml
Starting galaxy role install process
- downloading role 'docker', owned by geerlingguy
- downloading role from https://github.com/geerlingguy/ansible-role-docker/archive/7.0.2.tar.gz
- extracting geerlingguy.docker to /workspace/ansible/roles/geerlingguy.docker
- geerlingguy.docker (7.0.2) was installed successfully
```

```
vscode@d13c36f91cab:/workspace/ansible$ cat .envrc
export ANSIBLE_BECOME_PASS=<your ansible become pass>
```

```
vscode@d13c36f91cab:/workspace/ansible$ ansible -m ping -i inventories/dev/hosts.ini rancher
rancher-rocky-8-01 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/libexec/platform-python"
    },
    "changed": false,
    "ping": "pong"
}
```

```
vscode@d13c36f91cab:/workspace/ansible$ ansible -m ping -i inventories/dev/hosts.ini rancher
rancher-rocky-8-01 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/libexec/platform-python"
    },
    "changed": false,
    "ping": "pong"
}
```
