# Before start

We have two entities: our computer and the router.

## How does it work

1. We have the `wlan0` interface on our PC, which is used to connect to the router. The router has a local IP address, for example, `192.168.1.1`, with a netmask of 255.255.255.0 (also known as `/24`)

2. Using `iwd` and `iwctl`, we connect to the router and use a DHCP client to retrieve the router's IP address and netmask. Once this process is complete, in `ip addr show`, we will see an `inet` interface alongside `inet6`, which is used for proxying our local IP address to the router.