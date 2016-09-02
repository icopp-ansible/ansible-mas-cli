# ansible-mas-cli

Install the [`mas-cli`](https://github.com/argon/mas) utility and log in with it. Does nothing on non-macOS platforms.

## Role Variables

`apple_id` and `apple_id_password` will be prompted for if not supplied.

## Dependencies

* [icopp.homebrew](https://github.com/icopp/ansible-homebrew) (included as repository dependency)

## Example Playbook

```
  - hosts: all
    roles:
      - mas-cli
```

```
  - hosts: all
    roles:
      - role: mas-cli
        apple_id: xxxxx@xxxxx.xxxxx
        apple_id_password: xxxxx
```

## License

MIT
