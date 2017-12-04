[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-php7-fpm.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-php7-fpm)

# lifeofguenter.php7-fpm

This role will install PHP7 (cli) from custom built deb packages.

## Requirements

none

## Role Variables

```yaml
php7fpm_default: true

php7fpm_error_log: /var/log/php7-fpm/error.log

php7fpm_conf_memory_limit: 256M

php7fpm_conf_opcache_memory_consumption: 256

php7fpm_conf_apc_shm_size: 256M

php7fpm_version: 7.1.12-2

php7fpm_ext_apcu_version: 5.1.8-2

php7fpm_ext_imagick_version: 3.4.3-2

php7fpm_ext_igbinary_version: 2.0.5-2

php7fpm_ext_redis_version: 3.1.4-2

php7fpm_ext_iredis_version: 1.0.0-2

php7fpm_ext_memcached_version: 3.0.4-2
```

## Dependencies

none

## Example Playbook

```yaml

- hosts: servers
  roles:
    - { role: lifeofguenter.php7-fpm }
```

## License

Licensed under the MIT License. See the [LICENSE file](LICENSE) for details.

## Author Information

[Gunter Grodotzki](https://lifeofguenter.de)
