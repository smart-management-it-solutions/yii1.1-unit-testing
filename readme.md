## Yii 1.1 Sample Test

## Step 1
 Add composer.json in protected directory and run composer install
 ```
 {                                                                                                                                  
    "require" : {
        "phpunit/phpunit": "3.7.*",
        "phpunit/dbunit": "1.3.*@dev",
        "phpunit/phpunit-selenium": "1.2.*",
        "phpunit/phpunit-story": "dev-master",
        "phpunit/php-invoker": "dev-master"
    }
}
```
``` 
composer install
```

## Step 2

Add this line to `tests/boostrap.php`

```
require_once('../vendor/autoload.php');
```

## Step 3

Run phpunit

```
../vendor/bin/phpunit functional

```

```
PHPUnit 3.7.38 by Sebastian Bergmann.

Configuration read from /var/www/html/wp-test/protected/tests/phpunit.xml

SSSSSS

Time: 18 ms, Memory: 4.00MB

OK, but incomplete or skipped tests!
Tests: 6, Assertions: 0, Skipped: 6.
```