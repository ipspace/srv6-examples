# SRv6 with IS-IS

This lab topology describes an IS-IS network with SRv6 enabled on the edge routers. The edge routers advertise their SRv6 locators in IS-IS TLVs, but all three routers (being SRv6-aware) install routes to those SRv6 locators in their IPv6 routing tables.

![3-node SRv6 with IS-IS topology](../../images/intro-topology.png)

For general instructions on starting labs, connecting to devices, and generating reports with `netlab`, see the [_Using the Labs_](../../docs/use.md) document.
