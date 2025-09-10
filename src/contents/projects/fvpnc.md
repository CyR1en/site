---
title: fvpnc
description: An unofficial command-line client for Namecheap's FastVPN for Linux
poster: /projects/generic.webp
techstack:
  - Python
---


An unofficial command-line client for [Namecheap's FastVPN](https://fastvpn.com/) for Linux, written in Rust 🦀 🦀 🦀.

_`fvpnc` can also be used in macOS. However, you are limited to only `OpenVPN`. To take advantage of `WireGuard` or `IKEV2` download the official client for macOS_

### Usage:

```
Usage: fvpnc <COMMAND>

Commands:
  status      Status of the connection
  cities      List all available cities
  disconnect  Disconnect from a server
  connect     Connect to a server
  help        Print this message or the help of the given subcommand(s)

Options:
  -h, --help     Print help
  -V, --version  Print version
```
For now, `fvpnc` is using `OpenVPN` to connect to the server. `IKEV2` and `WireGuard` could be supported in the future.

#### Authentication
When you initially run `fvpnc`, it will ask for your credentials that could be found at [here](https://account.fastvpn.com/)

#### Connecting
Connecting to a server is fairly easy, you just simply need to know which city you want to connect to and set your protocol.
```
fvpnc connect --udp Dallas
```
The command above will connect us to the `Dallas` server

#### Disconnecting
Disconnecting to the server, you simply run the following command:
```
fvpnc disconnect
```