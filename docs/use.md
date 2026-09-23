# Using the Labs

The repository contains SRv6-focused _netlab_ lab topologies and related usage instructions. You can start your labs in GitHub Codespaces ([instructions from a similar project](https://evpn.bgplabs.net/4-codespaces/)), or [install netlab locally](https://netlab.tools/install/) or in a [cloud VM](https://netlab.tools/install/cloud/).

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/ipspace/srv6-examples)

To start a lab:

* Change the current directory to the lab directory
* Execute `netlab up` to start the lab with FRRouting containers (default settings) or `netlab up -d _device_` to start the lab with [another device supporting SRv6](https://netlab.tools/module/srv6/). You can also change the `NETLAB_DEVICE` environment variable to use a different device type for all labs in the current shell/session, for example:

```
$ export NETLAB_DEVICE=iosxr
```

* Connect to lab devices with `netlab connect _nodename_`.

Use these commands to create lab topology reports:

* **netlab report devices** -- nodes, node IDs, device types, and device images
* **netlab report wiring** -- lab nodes and links
* **netlab report addressing** -- lab addressing
* **netlab report isis-nodes** -- IS-IS routing
* **netlab report mgmt** -- Management access to lab devices
