# Resource Limits

> [Issue](https://github.com/abi-am/it-resources/issues/3)

For protecting server from overloading and defining memory limits for users we use cgroups and systemd slices.

```bash
cat /lib/systemd/system/user-.slice.d/11-memory.conf
[Slice]
MemoryMax=10G
```

For Processes we defining resource limits in `.service` definition (or override).

```bash
systemctl set-property rstudio-server.service MemoryMax=50G
```

### Resources

- https://www.kernel.org/doc/Documentation/cgroup-v1/memory.txt
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/resource_management_guide/sec-memory
- https://docs.oracle.com/cd/E37670_01/E37355/html/ol_memory_cgroups.html
- https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/resource_management_guide/sec-moving_a_process_to_a_control_group
- https://documentation.suse.com/sles/15-SP1/html/SLES-all/cha-tuning-cgroups.html