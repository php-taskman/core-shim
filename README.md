# PHP Taskman binary

## Installation

```php
php -r "copy('https://github.com/php-taskman/core-shim/releases/latest/download/taskman.phar', 'taskman.phar');"
php -r "copy('https://github.com/php-taskman/core-shim/releases/latest/download/sha1sum.txt', 'sha1sum.txt');"
php -r "if (hash_file('sha1', 'taskman.phar') === current(explode(' ', file_get_contents('sha1sum.txt')))) { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('taskman.phar');unlink('sha1sum.txt');} echo PHP_EOL;"
chmod +x taskman.phar
```
