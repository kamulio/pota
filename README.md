# Ubuntu LAMP Setup

Bash scripts to automatically setup LAMP server following best practices.

Current version: `lamp-ubuntu22.sh`

## How to use

  * Log in to your fresh Ubuntu server as root
  * Download the most recent version of the script: `wget https://raw.githubusercontent.com/kamulio/pota/master/lamp-ubuntu22.sh`
  * Change permissions: `chmod 755 lamp-ubuntu22.sh`
  * Run and follow prompts: `./lamp-ubuntu22.sh`

## What does this script do?

  * Checks that you are root
  * Set the hostname. In general it is a good idea to use the real domain for your site as hostname.
  * Update packages from repo
  * Install utility software, Apache, PHP and MySQL (see detailed list below)
  * Setup unattended upgrades
  * Change www-data user password, and allow shell access
  * Apache configuration (see details below)
  * PHP configuration
  * MySQL configuration
  * Configure log rotation
  * Setup automatic daily database dump and rotation
  * Setup basic firewall rules
  * Setup fail2ban
  * Setup mod_security

## Installed Software

  * Utility software:
    * curl
    * vim
    * openssl
    * git
    * htop
    * nload
    * nethogs
    * zip
    * unzip
    * sendmail
    * sendmail-bin
    * libcurl3-openssl-dev
    * psmisc
    * build-essential
    * zlib1g-dev
    * libpcre3
    * libpcre3-dev
    * memcached
    * fail2ban
    * iptables-persistent
  * Apache and modules
    * apache2
    * apache2-doc
    * apachetop
    * libapache2-mod-php
    * libapache2-mod-fcgid
    * apache2-suexec-pristine
    * libapache2-mod-security2
  * PHP 8.1
    * mcrypt
    * imagemagick
    * php8.1
    * php8.1-common
    * php8.1-gd
    * php8.1-imap
    * php8.1-mysql
    * php8.1-mysqli
    * php8.1-cli
    * php8.1-cgi
    * php8.1-zip
    * php-pear
    * php-auth
    * php-mcrypt
    * php-imagick
    * php8.1-curl
    * php8.1-mbstring
    * php8.1-bcmath
    * php8.1-xml
    * php8.1-soap
    * php8.1-opcache
    * php8.1-intl
    * php-apcu
    * php-mail
    * php-mail-mime
    * php8.1-memcached
    * php-all-dev
    * php8.1-dev
    * libapache2-mod-php8.1
  * MySQL
  * NodeJS 12


## Thank You. 
