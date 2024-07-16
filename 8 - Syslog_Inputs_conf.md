## In Deployment Server
```bash
sudo su - splunk
cd /opt/splunk/etc/deployment-apps/
mkdir TCRA_Syslog_Input_Configs
cd TCRA_Syslog_Input_Configs
mkdir local
cd local 
vi inputs.conf
```

### Add below configs for each file

```bash
[udp://514]
connection_host = ip
index = tcra_syslog_server_idx
sourcetype = tcra:syslog:log
```


