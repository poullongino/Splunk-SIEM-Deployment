## To find OS version:
```bash
cat /etc/os-release
```

## To find Disk partition:
df -kh

cd /opt/splunk
df -kh .

cd /opt/splunkdata
df -kh .

Get CPU Details:
lscpu

Get Memory Details:
free -h

To check whether splunk user is created:
id -u splunk
lslogins -u splunk

To check if the user is in sudo group as well
groups splunk

To check if /opt/splunk directory exists and owner of that directory:
ll /opt/

Verify if Ports are open:
Ports to be opened at OS Level & Network level Firewalls
	• 8000, 8089, 8088, 9997, 8065, 8181, 9887, 8191, 514, 9777
