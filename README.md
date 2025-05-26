# Minecraft Hosting with Kubernetes & Kustomize

A simple(?) personal project that leverages kubernetes manifests and some handy community tooling to host minecraft servers. Used to start learning some kubernetes and to simpify hosting multiple servers with some key features:

A hosted map instance, courtesy of [BlueMap](https://github.com/BlueMap-Minecraft/BlueMap)

Automatic domain based routing, and auto scale up/down as needed, courtesy of [mc-router](https://github.com/itzg/mc-router)

Automatic backups with [mc-backup](https://github.com/itzg/docker-mc-backup)

Servers themselves are using [docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) to simplify running with various configs

The process of setting up a server involves copying a few overlay files, replacing some hardcoded names, and twaking settings as needed. There are patch files for loading existing worlds and using custom jar files.

This was a weekend project, with the help of some AI to aid in debugging/initial concept, before refining further. There are probably still issues, and it might change quite a bit in the future, but for now it works.
