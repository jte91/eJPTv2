# VIA METASPLOIT
## Find Version
Choose module: auxiliary/scanner/mysql/mysql_version

## Brute Force to see whether we can find any legitimate credentials to access database server
choose module: auxiliary/scanner/mysql/mysql_login
  Set username to root to find passwords for the root user
  Set pass_file to wordlist

## Enumeration process
Choose module:  auxiliary/admin/mysql/mysql_enum

## MySQL SQL module (interact with server)
Choose module: auxiliary/admin/mysql/mysql_sql
  “Admin” means we will require credentials to run
  Use credentials found in login module
  Set SQL 
  Set SQL show databases;
  This options lets you use SQL commands to get info that you’re looking to gather

## Show tables in the databases 
Choose module: auxiliary/scanner/mysql/mysql_schemadump 
  Set credentials
  NOTE: You can check various info gathered from runs
    Services
    Loot
    Hosts
    Creds

# LOGIN MySQL
Mysql -h TARGET -u USER -p (enter password when prompted)
