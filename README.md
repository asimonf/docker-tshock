# docker-tshock
---------------

A simple docker container for running a TShock Terraria server including the
Infinite Chests v2.0 plugin.

## Installation
---------------

You can install the latest automated build by pulling the image from
the docker index.

```bash
docker pull asimonf/tshock:latest
```

## Quick Start
--------------

There are two volumes created:

* /opt/tshock-server/Terraria/Worlds
* /opt/tshock-server/tshock

The first one is for containing the worlds created.
The second one is for containing the configuration and data files.

If you wish to override the configuration or the starting worlds, you can mount
the volumes to a host folder and create the necessary files before starting the
container. You might also wish to link it to mysql, for example. 

The container also uses an enviroment variable to select the world file. The
environment variable is TERRARIA_WORLD.
