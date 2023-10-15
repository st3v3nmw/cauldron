<div align="center">
    <img src="assets/img/logo.png" width="100" />
    <h1>Cauldron</h1>
</div>

Cloud infrastructure for my open-source &amp; self-hosted apps. Deployed for pennies on a HA Kubernetes cluster on [OVH Cloud](https://www.ovhcloud.com/en/) 🚀.

## Servers

- _Specs:_ 1vCPU, 2GB RAM, 20GB SSD, 2GB Swap Memory, Ubuntu 23.04
- _Number of VPS:_ 10
- _Locations:_ Germany (4), France (3), Poland (3)
- _Provider:_ [OVH Cloud](https://www.ovhcloud.com/en/)
- _Cost:_ 10 * $0.98 per month (1 year offer!)

## Kubernetes Cluster

Deployed using [Microk8s](https://microk8s.io/). \
The cluster is highly available out of the box since MicroK8s automatically enables [high availability](https://microk8s.io/docs/high-availability) for clusters with three or more nodes.

The storage solution used is [OpenEBS](https://microk8s.io/docs/addon-openebs). The volumes are [replicated](https://openebs.io/docs#what-does-openebs-do) thrice for redundancy.

### Ingress

- _Tool_: Nginx
- _Host_: cauldron.stephenmwangi.com
- _Certificate Issuer_: [Let's Encrypt](https://letsencrypt.org/)
- _DNS_: 4 A records pointing to hosts in different regions for redundancy

### Hosted Apps

#### CouchDB

Used to sync Obsidian notes across my devices using the [Obsidian LiveSync plugin](https://github.com/vrtmrz/obsidian-livesync/blob/main/docs/setup_own_server.md).

### Credits

#### Logo

<a href="https://www.flaticon.com/free-icons/cauldron" title="cauldron icons">Cauldron icon/logo created by Freepik - Flaticon</a>
