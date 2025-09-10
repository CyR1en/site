---
title: Voxx
description: Voxx is a desktop/command-line, non-persistent, drop-in, public chat channel, where users can chat with other connected users with a degree of anonymity. Users could also host their own Voxx server to set up a communication medium for their own use cases.
poster: /projects/generic.webp
techstack:
  - Java
  - Python
---

Voxx is a desktop/command-line, non-persistent, drop-in, public chat channel, where users can chat with other connected users with a degree of anonymity. Users could also host their own Voxx server to set up a communication medium for their own use cases. [[source](https://github.com/CyR1en/Voxx)]

- [x] **Multi-Client Server**: It is critical that the server is able to serve and handle multiple clients that connect to the server.
- [x] **Reliable Connection**: The connection between the client and the server needs to be stable, and all the features like sending messages and getting updates must still work until the client disconnects from the sever.
- [x] **Robust Communication Protocol**: The communication between the server and the client must be straight forward and easy to understand.
- [x] **Deployable Clients**: Voxx clients that's easy to install for the end user/clients.
- [x] **Deployable Server:** Make it easy for users to be able to start their own voxx server for their own use case.


### [Voxx CLI Client](https://github.com/CyR1en/voxx-client-cli)

```
pip install voxx-cli
```

##### Usage

```
Usage: voxx-cli [options] <arg>

-h   --help                      show this help message and exit
-a   --address ADDRESS           voxx server address
-u   --user USERNAME             username to register as
-v   --version                   show program's version number and exit

```