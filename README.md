[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-prosody.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-prosody)

# Ansible Role: prosody

An Ansible role that installs prosody (xmpp server) on Debian-like systems.

## Requirements

none

## Role Variables

```yaml

prosody_domain:

prosody_log_level: warn

prosody_use_mysql: false

prosody_mysql_host: 127.0.0.1

prosody_mysql_port: 3306

prosody_mysql_user: prosody

prosody_mysql_password:

prosody_mysql_db: prosody

prosody_allow_registration: false

prosody_ssl_cert:

prosody_ssl_key:

prosody_ssl_ciphers:

prosody_ssl_protocol: tlsv1_1+

prosody_ssl_dhparam:

prosody_recaptcha_private_key:

prosody_recaptcha_public_key:

prosody_s2s_secure_auth: true

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
