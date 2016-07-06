About
=======

A little cookbooks for Engine Yard Cloud


### Prepare command line tool for uploading and applying cookbooks

```
$gem install engineyard
$ey login
$ey recipes upload
$ey recipes apply 
```

### How to debug

```
cookbooks/main/recipes/default.rb
```

When you do apply your custom cookbooks, EY instances run main/recipes/default.rb
And your cookbooks and dns.json are placed at /etc/chef-custom/*

You can see the logs at

```
/var/log/chef.custom.log
```

If you can run by yourself, you can use this command at a target instance

```
sudo /usr/local/ey_resin/bin/chef-solo -j /etc/chef-custom/dna.json -c /etc/chef-custom/solo.rb
```


List
--------

### custom_php_ini

add php.ini

### jenkins_on_util

install and run Jenkins at Util server

### thin

use thin for web app

msuper usage
--------------
check below
> ey-mini-cookbook/cookbooks/modern_cipher_nginx/ [https://github.com/huihe/ey-mini-cookbook/tree/master/cookbooks/modern_cipher_nginx]
