---
sidebar_position: 1
---

# Introduction
In this article we will go into more detail on how to create an alt:V server.

If you have any questions or other concerns, please search in the documentation or ask in our [Discord](https://discord.gg/yQvKgSs).

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

By default alt:V uses port 7788 (TCP & UDP) if no [CDN](~/articles/cdn.md) is used.<br/>
If you are using a CDN, only UDP is used.
The port can be changed in the [server.toml](../getting_started/configuration_files/server_configuration.md).

### Interesting Facts

These are facts and similarities seen across all servers.

- The average mid-tier server utilizes 6-42% of their CPU. This is based on players and other factors.
- The average mid-tier server has a player count of roughly 300-600 players at peak hours.
- The average mid-tier server has RAM usage less than 1.25GB.
- The average mid-tier server has around 8 cores.
- The average mid-tier server is clocked at 3.7ghz