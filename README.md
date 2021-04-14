This is a fork of the old and awesome mindmup (mindmup-legacy).

## Run on Windows Subsystem for Linux (WSL2)
To run docker on WSL2, make sure your system is ready by installing docker based on these instructions:

https://dev.to/bartr/install-docker-on-windows-subsystem-for-linux-v2-ubuntu-5dl7

You'll need to know the IP address of your WSL2 instance.
```
ifconfig
```
Look for the ip address for eth0. For example. 172.19.37.24


This repo is _only_ for running mindmup-legacy offline. From the Linux command prompt:

```
docker build -t ogmindmup .
docker run -p 5000:5000 ogmindmup
```

From a webbrowser (i.e. Firefox on the Windows 10 host), open the mindmup webpage using the IP address at port 5000.

You can open a .mup file from the local file system. These services are all running local, so data is not shared to a remote server.

## The online version of Mindmup
See https://github.com/davedf/mindmup for the real deal.
