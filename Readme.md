# Sqlite3 to mysql
- First (Dump data from your sqlite to dump.sql)

  `sqlite3 your.db .dump > dump.sql`
- Second (Convert your dump.sql to mysql.sql for MySQL)

  `$ cat dump.sql | python sqlite3tomysql.py > mysql.sql`
- Third (Import mysql.sql on MySQL)

  `mysql -u USERNAME -p`
  
  `mysql> CREATE DATABASE hoge CHARACTER SET utf8mb4;`
  
  `mysql> USE hoge;`
  
  `mysql> source /path/to/mysql.sql;`
