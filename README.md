# PHP Taskman binary

## Installation

```php
php -r "copy('https://github.com/php-taskman/core-shim/releases/latest/download/taskman.phar', 'taskman.phar');"
php -r "copy('https://github.com/php-taskman/core-shim/releases/latest/download/taskman.phar.sha1sum', 'taskman.phar.sha1sum');"
php -r "if (hash_file('sha1', 'taskman.phar') === file_get_contents('taskman.phar.sha1sum')) { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('taskman.phar');unlink('taskman.phar.sha1sum');} echo PHP_EOL;"
rm taskman.phar.sha1sum
chmod +x taskman.phar
mv taskman.phar taskman
```
