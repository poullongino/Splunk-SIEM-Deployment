## To find OS version:
```bash
cat /etc/os-release
```

## To find Disk partition:
```bash
df -kh
```

```bash
cd /opt/splunk
df -kh .
```

```bash
cd /opt/splunkdata
df -kh .
```

## Get CPU Details:
```bash
lscpu
```

## Get Memory Details:
```bash
free -h
```

## To check whether splunk user is created:
```bash
id -u splunk
lslogins -u splunk
```


## To check if /opt/splunk directory exists and owner of that directory:
```bash
ll /opt/
```

## Verify if Ports are open:
### Ports to be opened at OS Level & Network level Firewalls
	• 8000, 8089, 8088, 9997, 8065, 8181, 9887, 8191, 514, 9777

 ## Check if the THP is disabled
```bash
sudo cat /sys/kernel/mm/transparent_hugepage/enabled
sudo cat /sys/kernel/mm/transparent_hugepage/defrag
```

## Check if the ulimit is increased
```bash
ulimit -a splunk
```

