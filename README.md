# WP MU-Plugin: Hide Development/Testing enviroments from robots

Deny site from `/robots.txt` if it's accessed with `WP_ENV=staging` or `WP_ENV=testing`.

Also denys it if the site is accessed with domain that ends with domain mentioned in `WP_HIDE_ROBOTS_DOMAINS`.

## Installation
```
$ composer require alexsancho/wp-noindex-robots
```

## Example config
```php
// hides site from robots if its accessed from any geniem.io or example.com subdomain.
define( 'WP_HIDE_ROBOTS_DOMAINS', 'example.com,example.test' );
```
