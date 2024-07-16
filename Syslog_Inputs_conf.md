## In Deployer
```bash
sudo su - splunk
cd /opt/splunk/etc/deployment-apps/
mkdir TCRA_Syslog_configs
cd TCRA_Syslog_configs
mkdir local
cd local 
vi inputs.conf
```

### Add below configs for each file

```bash
[monitor:///var/log/messages]
disabled = 0
index = tcra_syslog_server_idx
sourcetype = tcra:syslog:log
interval = 60
```
