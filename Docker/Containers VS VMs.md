### General information
Docker containers offer lightweight containerization by sharing the host OS kernel unlike a VM; which runs a complete kernel, thus requiring more system resources. This sharing of a kernel allows for faster startup and smaller storage footprint compared to VMs. While this means you can only run containers of the same OS as your host (f.e., Windows 11 containers on Windows 11), VMs virtualize the entire machine, allowing different OSs but with slower startup and larger storage needs. Installing Windows Subsystem for Linux (WSL)(recommended) or having Hyper-V enabled allows the ability to Linux containers on Windows machines.

```mermaid
graph TB
    subgraph Container/Docker
    Application
    Bin/Libs
    Docker-Engine
    Host-OS
    Server
end
```

```mermaid
graph TB
    subgraph Virtual Machine
    Application
    Bin/Libs
    Guest/OS
    Hypervisor
    Host-OS
    Server
    
end
```

### Isolation
Virtual Machines offer complete isolation from the host OS and other VMs. Containers on the other hand does not provide as strong isolation, considered a more "lightweight" isolation.

More details and information can be found in the references section: 

---
### References
https://learn.microsoft.com/en-us/virtualization/windowscontainers/about/containers-vs-vm

https://www.atlassian.com/microservices/cloud-computing/containers-vs-vms
