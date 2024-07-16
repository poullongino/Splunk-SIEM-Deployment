### In Syslog server

```bash
cd /etc/syslog-ng
vi syslog-ng.conf
```

Add the below listed lines to forward the data.
Use your splunk instance IP address & Port number

```bash
source tcp_log {
  file("/var/log/secure");
};

destination splunk_tcp {
  network("35.179.4.112" transport("udp") port(5514));
};

log {
  source(tcp_log);
  destination(splunk_tcp);
};
```

