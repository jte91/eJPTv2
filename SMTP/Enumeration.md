# VIA METASPLOIT

## Find Version
Choose module: auxiliary/scanner/smtp/smtp_version

## Enum for User
Choose module: auxiliary/scanner/smtp/smtp_enum

# Nmap 

Find community strings:

Nmap -sU -p 161 –script=smb-brute demo.ine.local

Reable:

Nmap -sU -p 161 –script snmp-* demo.ine.local > snmp_info

Cat the file

# Snmp Walk to gather more info

Snmpwalk -v 1-c public demo.ine.local
