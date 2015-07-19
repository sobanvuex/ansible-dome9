# Dome9

Cloud Infrastructure Security.

## Role Variables

* `dome9_pair_key` - **Required**. Your paring key from [Dome9](https://dome9.com/).
* `dome9_server_name` - Custom name to use in Dome9. Defaults to `ansible_hostname`.
* `dome9_security_groups` - List of groups to pair with. Defaults to `['Default']`.
* `dome9_upgrade` - Boolean. Use it to perform a package upgrade.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: SobanVuex.dome9, dome9_pair_key: <your_dome9_pairing_key> }
```

## License

MIT
