# nagios-check-host
checks using nagios json api if host exist used for automation etc

### Usage

create a file named:
```nagioscredentials.py```

```
NAGUSER = '###'
NAGPWD = '###'
NAGURL = 'https://nagios.domain.com/nagios/cgi-bin/objectjson.cgi?query=host&hostname=%s'
```

## to check for host
nagios-check-host <hostname>

