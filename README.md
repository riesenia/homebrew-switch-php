# switch-php

Installs and switches between different versions of PHP (7.4, 8.1, and 8.3).

## Configuration

Add PHP modules to the *httpd.conf* file to load the correct PHP module for each version:

```
# Load PHP 7.4 Module
LoadModule php7_module /usr/local/opt/php@7.4/lib/httpd/modules/libphp7.so

# Load PHP 8.1 Module
LoadModule php_module /usr/local/opt/php@8.1/lib/httpd/modules/libphp.so

# Load PHP 8.3 Module
LoadModule php_module /usr/local/opt/php@8.3/lib/httpd/modules/libphp.so
```

Make sure these paths match the location of the PHP modules installed by Homebrew.

## Usage

```bash
switch-php 7.4
switch-php 8.1
switch-php 8.3
```
