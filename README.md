oro-vagrant-config
==================

Oro Vagrant configuration created with Puphpet

Requirements
--
- Virtual Box
- Vagrant >= 1.5.0

Configuration settings
--
## OS
- Debian Wheezy 7.2 x64
- Box IP 192.168.56.102
- Forwarded SSH port (host / box) 5276 / 22
- Synced folder ./ -> /var/www

## Apache 2.x
- Virtual Host oro.dev -> /var/www/oro/web
- User / group - vagrant

## PHP

### Version
- 5.4

### Modules
- cli
- intl
- mcrypt
- gd2
- curl
- xdebug

### Settings

- display_errors = On
- error_reporing = -1
- memory_limit = 512M
- short_open_tag = Off
- max_execution_time = 300
- xdebug.remote_enable = 1
- xdebug.remote_port = 9000
- xdebug.max_nesting_level = 300

## MySQL 5.5
- username = orocrm
- database = oro_crm
- password = 123
- root password = 123

## NodeJS
- v0.10.26
- npm v1.4.3

## MailCatcher
- HTTP port 1080
- SMTP port 1025
- log /var/log/mailcatcher/
