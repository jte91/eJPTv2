# VIA METASPLOIT
## Find SMB Version
Choose module: auxiliary/scanner/smb/smb_version
  For the results look at what is in the "()"

## Find SMB Users
Choose module: auxiliary/scanner/smb/smb_enumusers

## Find Shares
Choose module: auxiliary/scanner/smb/smb_enumshares
  set ShowFiles true

## Brute Forcing 
Choose module: auxiliary/scanner/smb/smb_login

Hydra -l admininstrator -P /usr/share/wordlists/metasploit/unix_users.txt TARGET smb

# Log in

smbclient -L TARGET -U USER

smbmap -u USER -p PASS -H TARGET

## Check if User exist 

smbclient //TARGET/user -U USER

