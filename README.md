# Rustdesk
[RustDesk](https://rustdesk.com/docs/en/) is one of my remote desktop applications. I have decided to self host the [RustDesk Open Source Server](https://rustdesk.com/docs/en/self-host/rustdesk-server-oss/). The server keeps a directory of all the hosts that I work with.  It is a discover and a security server.

I decided that I want to self host.  The [instructions](https://rustdesk.com/docs/en/self-host/rustdesk-server-oss/docker/) are pretty straight forward, running as two docker containers. The `docker-compose.yml` is almost verbatium that same as the example one.  I am running the server behind a NAT firewall, and I openned the [recommended ports](https://rustdesk.com/docs/en/self-host/rustdesk-server-oss/docker/#requirements). 
Note:  the data directory holds an sqlite database and a public/private key pair.  The public key needs to be added to each RustDesk host's client software.

I found the following article very helpful for configuring the RustDesk clients. 
- [Building Your Own Remote Desktop Solution: RustDesk Self-Hosted on Cloud with Docker](https://www.linkedin.com/pulse/building-your-own-remote-desktop-solution-rustdesk-cloud-montinaro-bv94f)
