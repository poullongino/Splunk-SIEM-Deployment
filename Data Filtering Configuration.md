Steps to filter the required events

1. Edit props.conf
   
```bash
[source::/var/log/messages]
TRANSFORMS-set= setnull,setparsing
```

2. Edit transforms.conf
   
```bash
[setnull]
REGEX = .
DEST_KEY = queue
FORMAT = nullQueue

[setparsing]
REGEX = \[sshd\]
DEST_KEY = queue
FORMAT = indexQueue
```

3. Restart the Splunk
