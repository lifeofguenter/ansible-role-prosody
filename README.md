[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-prosody.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-prosody)

# Ansible Role: prosody

An Ansible role that installs prosody (xmpp server) on Debian-like systems.

## Requirements

none

## Role Variables

```yaml

prosody_domain:

prosody_use_mysql: false

prosody_mysql_host: 127.0.0.1

prosody_mysql_port: 3306

prosody_mysql_user: prosody

prosody_mysql_password:

prosody_mysql_db: prosody

prosody_allow_registration: false

prosody_cert_path:

prosody_cert_key:

prosody_recaptcha_private_key:

prosody_recaptcha_public_key:

```

## Dependencies

none

## Example Playbook

```yaml

- hosts: xmpp
  roles:
    - { role: lifeofguenter.prosody }
```

## License

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

[Gunter Grodotzki](https://lifeofguenter.de)
