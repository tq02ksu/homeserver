# homeserver
Distributed Home Server Application Beyond NAS.

## Motivations
* Kubernetes based system become to normal nowadays. Especially, k3s is amazing software which can run many applications in a chip hardware box. As times going, we have some spard hardwares can use.
* FreeNas and TreeNas, etc opensource product uses traditional server client architecture, need a external IP address and large bandwidth for better work, that is hard to archive.
* FreeNas and TreeNas supports docker and k3s, but do not use docker itself, so that choose to refuse updating operation system, that is sometimes not make sense.
* WireGuard do not support communicating between hosts behind NAT, ZeroTier, Tailscale and other solutions are hard to use in China.


## Design
* Distributed architecture, uses a slim hardware as a home server, can configure other distributed servers like aws/alicloud host as slaves and fully control these servers, autoconfigure for collabrate work.
