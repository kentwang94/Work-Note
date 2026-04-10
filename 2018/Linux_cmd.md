# Linux cmd Cheat Sheet

## Common

```sh
# current path
pwd


```





## Installation

### Install Java on Linux

Some tutorials: [#1](https://thishosting.rocks/install-java-ubuntu/)

```bash
java -version  # Check current version

```



## Utilities

### Native

```sh
# Monitor running processes' status (CPU/Mem) usage
top

# Dump internet usage info
tcpdump -i eth0 | less

```



### Third Party

```sh
# Monitor internet usage: use bmon
sudo apt-get install bmon
bmon


```

