### In Deployment Server

```bash
cd /opt/splunk/etc/deployment-apps/
mkdir TCRA_Forwarders_Outputs
cd TCRA_Forwarder_Outputs
mkdir local
cd local
vi outputs.conf
```

Paste below contents

```bash
[tcpout]
defaultGroup=intermediate_forwarders

[tcpout:intermediate_forwarders]
server=your_intermediate_forwarder1_ip:9997, your_intermediate_forwarder2_ip:9997
```
