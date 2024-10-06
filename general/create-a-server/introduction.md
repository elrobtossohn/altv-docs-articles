---
sidebar_position: 1
---

# Introduction
In this article we will go into more detail on how to create an alt:V server.

If you have any questions or other concerns, please search in the documentation or ask in our [Discord](https://discord.gg/altv).

## FAQ

### Which server specifications should I meet?

According to some statistics, these requirements are best suited for up to 100 players:
- CPU 3.2ghz
- 4 Cores
- 4 GB of RAM (Additional for Databases, etc.)
- Disk Space (Depends on Database and Script)

:::info

These requirements vary depending on the performance of the scripts and upcoming features.

:::

### Which ports are used?

By default alt:V uses port 7788 (TCP & UDP) if no [CDN](../../utilities/cdn_links.mdx) is used.<br/>
If you are using a CDN, only UDP is used.
The port can be changed in the [server.toml](../getting_started/configuration_files/server_configuration.md).

### Interesting Facts

These are facts and similarities seen across all servers.

- The average mid-tier server utilizes 6-42% of their CPU. This is based on players and other factors.
- The average mid-tier server has a player count of roughly 300-600 players at peak hours.
- The average mid-tier server has RAM usage less than 1.25GB.
- The average mid-tier server has around 8 cores.
- The average mid-tier server is clocked at 3.7ghz



### Worker ports

We recommend activating this feature with a player count of 500, as it serves as a "load balancer".

You can easily activate this feature by making the following entry in the [server.toml](../getting_started/configuration_files/server_configuration.md):
```toml
worker-ports = [7789, 7790]
```

#### When do you recommend using it?
We have created a simple formula, add an extra port for every 500 players. This means
500+ players: two worker ports
1000+ players: three worker ports
1500+ players: four worker ports

#### Does this affect my network infrastructure?
Yes, this change may affect your DDOS protection, you should check with your provider. The additional ports only require UDP, the default port still requires TCP.
