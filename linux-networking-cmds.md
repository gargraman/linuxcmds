### Active network connections, routing information, and other network statistics
```
netstat -ant
```

### Displays the path and hops that packets take to reach a remote server.
```
ping 8.8.8.8
```

### DNS lookups to resolve hostnames, IP addresses
```
nslookup example.com
```

### DNS lookups to query information about DNS name servers.
```
dig @8.8.8.8 example.org 
```

### Mac port listen
```
lsof -i -P | grep LISTEN 
```
OR
```
netstat -anvp tcp | awk 'NR<3 || /LISTEN/'
```
