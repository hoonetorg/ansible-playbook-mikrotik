# ansible-playbook-mikrotik

Runs ansible-role-mikrotik against the hosts in group `routeros` (full configuration deployment,
see the role README).

## Usage

```bash
ansible-playbook -i <inventory> -k --ask-vault-password site.yml -l <device>
```

`ansible.cfg` sets the roles path, log path and paramiko options for RouterOS connections.

## License

Apache-2.0

Created with the help of AI
