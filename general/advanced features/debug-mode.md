---
title: Debug Mode
sidebar_position: 0
---

## What is the debug mode?

The debug mode is a feature for developers to work on their scripts.<br/>
However, errors can occur such as some objects, interiors, vehicles or other things no longer being visible.

Players who do have debug mode enabled can only connect to servers where debug mode is enabled.<br/>
Players who do not have debug mode enabled can connect to servers where debug mode is enabled or disabled.

## Usage

To activate debug mode, you must add the following entry in the [client configuration](../getting_started/configuration_files/client_configuration.md) or the [server configuration](../getting_started/configuration_files/server_configuration.md):<br/>
You can also [click here](altv://action/setcfg?debug=true) to add the entry to the client.

```toml
debug = true
```

Debug mode is activated after a restart of the server or client.

:::tip Reminder

Debug mode should not be activated on a production server.

:::

## FAQ / Known issues

### How do i disable the debug mode?

[Click here](altv://action/setcfg?debug=false) to disable the debug mode.

### After reconnecting to the server some models or interiors aren't loaded

The reconnect command or feature was developed to make it easier for developers to work on their script.<br/>
Many things are not unloaded from the cache when reconnecting, which can lead to crashes but also to unloaded objects (vehicles, interiors etc.).