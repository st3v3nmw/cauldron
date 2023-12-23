<div align="center">
    <img src="assets/img/logo.png" width="100" />
    <h1>Cauldron</h1>
</div>

Kubernetes infrastructure for my open-source &amp; self-hosted apps 🚀.

## Nodes

| Host  | CPU               | RAM             | Operating System    | Role         | Description                                    |
| ----- | ----------------- | --------------- | ------------------- | ------------ | ---------------------------------------------- |
| mars  | 3 @ 2.8GHz (vCPU) | 4GB + 4GB Swap  | Ubuntu Server 22.04 | Control Pane | VPS from [Alwyzon](https://www.alwyzon.com/en) |
| luna  | 4 @ 2.00GHz       | 8GB + 8GB Swap  | Ubuntu Server 22.04 | Worker       | Old laptop                                     |

## Kubernetes Cluster

Deployed using [Microk8s](https://microk8s.io/).

The nodes are connected together using [Tailscale](https://blog.jaredallard.me/microk8s-and-tailscale/).

The storage solution used is [Longhorn](https://longhorn.io/).

### Ingress

- _Tool_: Nginx
- _Root host_: cauldron.stephenmwangi.com
- _Certificate Issuer_: [Let's Encrypt](https://letsencrypt.org/)

### Hosted Apps

#### [Postgres](https://www.postgresql.org/)

The world's most advanced open source relational database.

#### [Redis](https://redis.io/)

The open source, in-memory data store used by millions of developers as a database, cache, streaming engine, and message broker.

### Credits

#### Logo

<a href="https://www.flaticon.com/free-icons/cauldron" title="cauldron icons">Cauldron icon/logo created by Freepik - Flaticon</a>
