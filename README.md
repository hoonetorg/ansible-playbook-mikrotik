# ansible-playbook-mikrotik

Runs ansible-role-mikrotik against the hosts in group `routeros` (full configuration deployment,
see the role README).

## Usage

```bash
ansible-playbook -i <inventory> -k --ask-vault-password site.yml -l <device>
```

Uses the `ansible.cfg` of the nsbldr container (paramiko `look_for_keys = False` is required for RouterOS).

## License

Apache-2.0

Created with the help of AI
