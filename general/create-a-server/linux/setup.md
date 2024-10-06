---
title: Setup
sidebar_position: 1
---

### Before installation

Before we can really get started, you should create a user.  
We use “altv" as the user in the article, but you can choose your own name.

Simply enter the following command in a terminal: `adduser altv`  
Then switch to this user using `su altv`

:::warning

The server should never run with the "root" user.

:::

In the following steps, we will install and start the server.  
We use `/home/altv/server` as the directory, but you are free to choose your own directory.

Create and go to the `/home/altv/server` directory:
1. `mkdir -p /home/altv/server`
2. `cd /home/altv/server`

### Download (Using altv-pkg)

Visit the [alt:V Downloads page](https://altv.mp/downloads/) and scroll down to the server selection.  
Select `altv-pkg` in the tab and follow the instructions.

### Download & Upload (Using FTP)

Visit the [alt:V Downloads page](https://altv.mp/downloads/) and scroll down to the server selection.

1. Select **Linux x64** under `Server OS`.
2. Under Modules you can now select everything you need.  
   2.1 You do not have to select all modules, as a beginner we recommend the **JS Module** (JavaScript Module).
3. Select `Data files` and `Sample server config`.  
   3.1 The item “Example resource pack" is not relevant.
4. Click on **Download Server** to download the Server.

#### Upload
1. Connect to your server with an FTP client (We recommend [WinSCP](https://winscp.net/eng/docs/getting_started))
2. Go to `/home/altv/server` and upload the **altv-server.zip**
3. Unpack the archive with `unzip -q altv-server.zip`

### Set the permission

Use now `chmod +x altv-crash-handler` and `chmod +x altv-server`

### Start the server

To start the server, you can simply use `./altv-server`