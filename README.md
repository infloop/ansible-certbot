# ansible-certbot
Ansible certbot role

An Ansible role that generates new Let's Encrypt certificates

## Requirements

None

## Role Variables

- `certbot_enable` (boolean: true|false), default: `true`
- `certbot_webroot_path_path` (string), default: `/tmp/letsencrypt-webroot-share/`
- `certbot_admin_email` (string), default: `email@example.com`
- `certbot_certs` (array) default: []
  ```
  
  ```

- `generated_certs_copy` (boolean: true|false), default: `false`
- `generated_certs_copy_path` (string), default: `''`

## Dependencies

SSHF installed locally.

## Example Playbook

    - hosts: servers
      roles:
         - { role: infloop.ansible-certbot }
         
## Example Requirements

    - name: infloop.ansible-certbot
      src: https://github.com/infloop/ansible-certbot
      version: origin/master

## License

MIT