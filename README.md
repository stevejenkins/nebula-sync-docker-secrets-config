# Compose File for nebulas-sync with Docker Secrets
Easy Docker compose file for [nebula-sync](https://github.com/lovelaze/nebula-sync) with Docker Secrets support for quick and easy synchronization of multiple [Pi-hole](http://pi-hole.net) ad blockers.

## Before You Start
- Make sure you have at least two (2) fully-functional Pi-hole servers.
- Verify you know the port number(s) of all Pi-hole servers' web interfaces. Common ones are :80, :443, :8080, :8089, etc.
- Select one (1) Pi-hole server as your *Primary* server.
- The remaining Pi-hole server(s) will be *Replicas* of the Primary.
- Make sure your network is configured so that the server that runs Docker can ping/access the IP addresses of all Replicas. Most users run Docker (and thererefore the nebula-sync container) on the same server as the Primary Pi-hole, but it's not required. Any Docker host that can ping/access all the Pi-holes you wish to syncronize will work... even if that Docker host isn't running Pi-hole.

## Step 1: Clone this Repository to your Docker host
```git clone https://github.com/stevejenkins/nebula-sync-docker-secrets-config.git /opt/nebula-sync```

```nano /opt/nebula-sync/secrets/primary.txt```

Replace http://123.123.123.123:8049 with IP address or hostname of the Primary Pi-hole.
## Step 2: Configure API access to your Pi-holes




## Step 3: Configure your Docker Secrets files
If you plan to using Docker Secrets (recommended), you won't need to edit the included ```compose.yaml``` file at all. You simply need to include the 

