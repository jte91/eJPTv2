# VIA METASPLOIT
## Search Web Server Version
Choose module: auxiliary/scanner/http/http_version

## Enumerate HTTP Header
Choose module: auxiliary/scanner/http/http_header

## Enumerate by downloading robots.txt file
Choose module: auxiliary/scanner/http/robots_txt
curl out info that is found 

## Directory Brute Force
choose module: auxiliary/scanner/http/dir_scanner
curl into directories to see contents

## Search files in directory
choose module: auxiliary/scanner/http/files_dir

## Enumerate Users
choose module: auxiliary/scanner/http/apache_userdir_enum
set: 
  USER_FILE 
  
## Login module
choose module: auxiliary/scanner/http/http_login
set:
  AUTH_URI to directory
  Unset USERPASS_FILE if you already have a PASS_FILE and USER_FILE
  Set those credential files something more strong if need be

# VIA CMD

## Directory Busting 
#### Use Dirb
dirb http://IP_ADDESS -u USER:PASS
