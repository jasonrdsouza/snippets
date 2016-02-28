# Formatting and Mounting an EBS Volume

```bash
# View available disk devices and their mount points
~$ lsblk
# Check if the device already has a file system
~$ sudo file -s /dev/xvdb
# If there is no file system, create one like so
~$ sudo mkfs -t ext4 /dev/xvdb
# Create a mount point, and mount the volume
~$ sudo mkdir /data
~$ sudo mount /dev/xvdb /data
# Check that the volume was mounted properly
~$ df -h
```

Don't forget to change permissions/ ownership of the mount point depending on
who/ what needs to write to it.

