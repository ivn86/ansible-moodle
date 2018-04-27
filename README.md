ivn86.moodle
============

+ install moodle on Centos 7
+ instal dependencies: nginx, php7, mariadb

Requirements
------------

+ Centos 7

Role Variables
--------------

```
moodle_download_url: "https://download.moodle.org/download.php/direct/stable34/moodle-latest-34.tgz"

www_path: "/home/www"
www_user: nginx
www_group: nginx

domain_name: "www.example.com"

mysql_db: moodle
mysql_user: moodle
mysql_pass: M00d13

moodledata_path: "/home/www/moodledata"
```

Dependencies
------------

No specific dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ivn86.moodle, mysql_pass: SomeStrongPassw0rd }

License
-------

BSD

Author Information
------------------

Ivan Zharenkov <ivan@zharenkov.ru>
