# Tailscale

[Homepage](https://tailscale.com/)

## Status
Active

## License
BSD

## Clients
* Linux
* Android
* iOS
* Windows
* MacOS
* BSD?

## Servers
* The only official server is the proprietary one run by Tailscale.
* [Headscale](https://github.com/juanfont/headscale) (unofficial but also contributed to by official devs).

## Self-Hosting
Third party only.
The official servers are the proprietary ones run by the company Tailscale, but there is a third party open source server (Headscale) that works with the official clients.

## OSI Layer[s]
* 3

## NAT Traversal
Yes. A server somewhere that the clients can connect to directly is required no matter what so there is always a common point of contact to coordinate hole punching.

## Routing/Firewall
* Does it route directly peer to peer?
	* Yes.
* Does it create a mesh?
	* No.
* Does it isolate groups of clients/servers?
	* Yes - Groups of clients are managed by a user and access between groups and between users is very very limited.
* Does it filter access to ports based on the origin?
	* No.

## Setup Notes
* Piping scripts from the web to the shell is gross but it does make for a really easy install on supported distros.
* The client for android is also really easy to setup and connect.
* The connection process (assuming you already have an account) consists of clicking a link and signing into the server.
* Connecting to Headscale is a little more involved but only a tiny bit.

## Performance
* Better than Tinc by a little but not as good as plain Wireguard.

### Speed
Not benchmarked here yet.

### Notes
* Cheats by using a rock solid protocol somebody else wrote. /s

## Notes
* A very nice free tier is available for the hosted server.
* It's unfortunate that the official server isn't opensource even if they were to license it in a way that wasn't FOSS.* The data doesn't traverse the servers as long as the two peers can manage to poke their way through arbitrary layers of NAT.
* There are two types of servers.
	* Coordinating servers that just orchestrate connections
	* DERP servers that proxy data when clients can't connect directly after punching holes.
* The client always uses the wireguard-go implementation so performance isn't always great.

