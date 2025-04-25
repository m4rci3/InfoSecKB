Container networking refers to the ability for containers to connect to and communicate with each other, or to non-Docker workloads.

Containers have networking enabled by default, and they can make outgoing connections. A container has no information about what kind of network it's attached to, or whether their peers are also Docker workloads or not. A container only sees a network interface with an IP address, a gateway, a routing table, DNS services, and other networking details. That is, unless the container uses the none network driver.

### Drivers

The following network drivers are available by default, and provide core
networking functionality:

| Driver | Description |
| --- | --- |
| `bridge` | The default network driver. |
| `host` | Remove network isolation between the container and the Docker host. |
| `none` | Completely isolate a container from the host and other containers. |
| `overlay` | Overlay networks connect multiple Docker daemons together. |
| `ipvlan` | IPvlan networks provide full control over both IPv4 and IPv6 addressing. |
| `macvlan` | Assign a MAC address to a container. |

Docker bridge network isolation: Docker’s bridge network is a private, internal network that connects containers. External devices on the LAN don’t belong to this network, so those external devices cannot access the docker containers themselves, instead through the host device because of the nature of this driver type.
