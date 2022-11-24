# Drupal deploy

This repo is going to have a docker-compose to deploy Drupal with nginx using the bitnami image


Info will be added


## Just for reference atm (will be deleted from here)
[Available environment variables:](https://github.com/bitnami/containers/tree/main/bitnami/drupal-nginx#user-and-site-configuration)
User and Site configuration

    DRUPAL_PROFILE: Drupal installation profile. Default: standard
    DRUPAL_SITE_NAME: Drupal blog name. Default: My blog
    DRUPAL_SKIP_BOOTSTRAP: Whether to skip performing the initial bootstrapping for the application. Default: no
    DRUPAL_ENABLE_MODULES: Comma or space separated list of installed modules to enable during the first initialization. No defaults.
    DRUPAL_USERNAME: Drupal application username. Default: user
    DRUPAL_PASSWORD: Drupal application password. Default: bitnami
    DRUPAL_EMAIL: Drupal application email. Default: user@example.com
    DRUPAL_CONFIG_SYNC_DIR: Drupal sync configuration directory location. Only used when DRUPAL_SKIP_BOOTSTRAP is enabled. No defaults.
    DRUPAL_HASH_SALT: Drupal string used to generate random values. Only used when DRUPAL_SKIP_BOOTSTRAP is enabled. No defaults.

Use an existing database

    DRUPAL_DATABASE_HOST: Hostname for MariaDB server. Default: mariadb
    DRUPAL_DATABASE_PORT_NUMBER: Port used by MariaDB server. Default: 3306
    DRUPAL_DATABASE_NAME: Database name that Drupal will use to connect with the database. Default: bitnami_drupal
    DRUPAL_DATABASE_USER: Database user that Drupal will use to connect with the database. Default: bn_drupal
    DRUPAL_DATABASE_PASSWORD: Database password that Drupal will use to connect with the database. No defaults.
    DRUPAL_DATABASE_TLS_CA_FILE: TLS CA certificate for connections. No defaults.
    ALLOW_EMPTY_PASSWORD: It can be used to allow blank passwords. Default: no

SMTP Configuration

To configure Drupal to send email using SMTP you can set the following environment variables:

    DRUPAL_SMTP_HOST: SMTP host.
    DRUPAL_SMTP_PORT: SMTP port.
    DRUPAL_SMTP_USER: SMTP account user.
    DRUPAL_SMTP_PASSWORD: SMTP account password.
    DRUPAL_SMTP_PROTOCOL: SMTP protocol. (standard, tls, ssl).

PHP configuration

    PHP_ENABLE_OPCACHE: Enable OPcache for PHP scripts. No default.
    PHP_EXPOSE_PHP: Enables HTTP header with PHP version. No default.
    PHP_MAX_EXECUTION_TIME: Maximum execution time for PHP scripts. No default.
    PHP_MAX_INPUT_TIME: Maximum input time for PHP scripts. No default.
    PHP_MAX_INPUT_VARS: Maximum amount of input variables for PHP scripts. No default.
    PHP_MEMORY_LIMIT: Memory limit for PHP scripts. Default: 256M
    PHP_POST_MAX_SIZE: Maximum size for PHP POST requests. No default.
    PHP_UPLOAD_MAX_FILESIZE: Maximum file size for PHP uploads. No default.
