##About
Script using nagios json api to check if host exist in nagios.

## Prerequisite

create a file named ```nagioscredentials.py``` with below content:

```
NAGUSER = 'nagiosuser'
NAGPWD = 'nagiospass'
NAGURL = 'https://nagios-server.mydomain.com/nagios/cgi-bin/statusjson.cgi?query=host&hostname=%s'
EXTENDED_STATUS = True
```

``Note``: Chang credentials and link reference according to your enviroment...

## Usage example
nagios-check-host  "hostname.domain.com"
