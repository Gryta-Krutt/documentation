---
description: This page discusses potential solutions to endpoint issues
---

# 🤝 Handshake issues

## Incorrect or unreachable address

### Incorrect address

Double check that the address you are attempting to connect to is correct. Usually an ip-address and port will look like this: `127.0.0.1:2700`. If you are connecting directly, using an IP-address as shown, make sure to include the specific **port** (the `2700`) you wish to connect to. If you are using a hostname then the port should not be added. A hostname can look like this: `wss://socket.gryt.net`.

### Check reachability

You can check if the address is reachable by opening a terminal (cmd on windows) and executing the following command:

```bash
telnet <ip_address> <port_number>
```

Replace `ip_address` and `port_number` with the appropriate values and check to see if you are receiving a pong back. **The default port number is 2700**

If you are receiving _connection refused_ it means the server **** is **not reachable.** This can occur either because:\
A) The server is not open to the public (server's port is closed)\
B) You wrote the incorrect ip-address or port\
C) Your internet connection is unstable _(very unlikely)_

#### Example of <mark style="color:green;">reachable</mark> endpoint

```
sivert@Siverts-MBP ~ % telnet localhost 2700
Trying ::1...
Connected to localhost.
Escape character is '^]'.
^CConnection closed by foreign host.
```

#### Example of <mark style="color:red;">unreachable</mark> endpoint

```
sivert@Siverts-MBP ~ % telnet localhost 3521
Trying ::1...
telnet: connect to address ::1: Connection refused
Trying 127.0.0.1...
telnet: connect to address 127.0.0.1: Connection refused
telnet: Unable to connect to remote host
```

#### command not found: telnet

If you are on **macOs** and the telnet command is not found, try installing it using brew first:

```bash
brew install telnet
```
