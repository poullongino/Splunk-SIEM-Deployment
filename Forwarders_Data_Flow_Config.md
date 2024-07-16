### In Intermediate forwarder UI
  Enable receiving - Settings >> Forwarding and receiving >> Configure receiving >> Add new >> 9997
    - Repeat the same procedure on both Intermediate Forwarders


### In Deployment Server backend

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


### In Deployment Server UI

Create a server class named "Data Source Forwarder Outputs" & Assign the App "TCRA_Forwarder_Outputs", Assign the Forwarder client 
