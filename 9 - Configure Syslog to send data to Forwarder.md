### In Syslog server

```bash
cd /etc/syslog-ng
vi syslog-ng.conf
```

Add the below listed lines to forward the data.
Use your splunk instance IP address & Port number

```bash
source s_network{
  udp();
};

destination splunk_udp {
  network("127.0.0.1" transport("UDP") port(514));
};

log {
  source(s_network);
  destination(splunk_udp);
};
```

