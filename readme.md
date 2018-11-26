

## Replace text/string in large file on your mac

```
sed -i '' 's/old-string/new-string/g' yourlargefile.sql
```


## Laravel Artisan Debug
Artisan command gives no results?
Put the code below in your artisan file, after opening the <?php and start debugging.
In most cases it will be a syntax error, related to you php version. 
See what php version you running "php -v" and check you composer file for 
which PHP version the framework needs.

```
ini_set('display_errors',1);
error_reporting(-1);
```    
