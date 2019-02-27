# Tcpdump

To make the output legible, as well as manageable, make sure to
1. specify the port you care about
2. use the -XX and -i flags to get ascii output next to the binary

```
sudo tcpdump -XX -i eth0 port 44380 > /tmp/dump
```
