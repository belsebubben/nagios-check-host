## About
Script using nagios json api to check if host exist in nagios.

## Prerequisite

create a file named ```nagioscredentials.py``` with below content:

```
NAGUSER = 'nagiosuser'
NAGPWD = 'nagiospass'
NAGURL = 'https://nagios-server.mydomain.com/nagios/cgi-bin/statusjson.cgi?query=host&hostname=%s'
EXTENDED_STATUS = True
```

``Note``: Change credentials and link reference according to your enviroment...

## Usage example
```
[j0nix]$ nagios-check-host super-server-1
2017-08-20 21:28:23,992 INFO: Success, super-server-1 found, status: up, checks_enabled: True, last_update: Sun Aug 20 21:28:13 2017
```

