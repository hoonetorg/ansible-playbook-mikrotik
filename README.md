# ansible-playbook-mikrotik

Runs ansible-role-mikrotik against the hosts in group `routeros` (full configuration deployment,
see the role README).

## Usage

```bash
ansible-playbook -i <inventory> -k --ask-vault-password site.yml -l <device>
```

Uses the `ansible.cfg` of the nsbldr container: `network_cli` connects with libssh (ansible-core 2.21 has no
paramiko connection anymore), `[libssh_connection] look_for_keys = False` is required for RouterOS
(password login without trying keys).

## License

Apache-2.0

Created with the help of AI
