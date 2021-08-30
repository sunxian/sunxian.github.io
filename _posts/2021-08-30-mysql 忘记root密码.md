---
layout: post
title:  "mysql 忘记root密码"
description: "mysql 忘记root密码，mariaDB忘记root密码"
date:   2021-08-30 12:52:00 +0800
categories: mysql,mariaDB
tags: [mysql, mariaDB]
---
#  mysql 忘记root密码

1. 停止mysql进程
2. mysqld_safe --skip-grant-tables &
3. mysql
4. use mysql;
5. FLUSH PRIVILEGES;
6. ALTER USER 'root'@'localhost' IDENTIFIED BY 'MyNewPass';

参考文档：

 https://dev.mysql.com/doc/refman/8.0/en/resetting-permissions.html

![image-20210830123152440](\assets\images\image-20210830123152440.png)