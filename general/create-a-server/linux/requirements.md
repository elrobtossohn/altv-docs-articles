---
title: Requirements
sidebar_position: 1
---

To install an alt:V server on Linux, the following minimum requirements should be met:
- A server that meets the [server specifications](../introduction.md#which-server-specifications-should-i-meet)
- The latest (and up-to-date) version of your Linux distribution
- libatomic1 (For most systems: `apt install libatomic1`)

If you plan to install the C# module, you will need:
- Latest [.NET 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0). ([.NET 9](https://dotnet.microsoft.com/en-us/download/dotnet/9.0) is also supported)

:::info

The standard version for the C# module is [.NET 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0), for higher versions the `AltV.Net.Host.runtimeconfig.json` must be modified.

:::