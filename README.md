# Ansible Role: PHP-PostgreSQL

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Installs PHP [PostgreSQL](https://www.postgresql.org/) support on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    php_enablerepo: ""

(RedHat/CentOS only) If you have enabled any additional repositories (might I suggest nholuong.repo-epel or nholuong.repo-remi), those repositories can be listed under this variable (e.g. `remi,epel`). This can allow you to install later versions of PHP packages.

    php_pgsql_package: php-pgsql # RedHat
    php_pgsql_package: php7.0-pgsql # Debian

The PHP PostgreSQL package to install via apt/yum. This should only be overridden if you need to install a unique/special package for PostgreSQL support, as in the case of using software collections on Enterprise Linux.

## Dependencies

  - nholuong.php

## Example Playbook

    - hosts: webservers
      roles:
        - nholuong.postgresql
        - nholuong.php
        - nholuong.php-pgsql

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟
