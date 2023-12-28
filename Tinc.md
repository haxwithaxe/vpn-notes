# Tinc v1.1

[Homepage](https://www.tinc-vpn.org/)

## Status
Unknown - Not officially dead but it sure looks like it is.

## License
GPLv2

## Clients
* If it is capable or running Linux of some kind there is probably a client for it even if it isn't currently running Linux. 
  * 
* Android
	* [TincApp](https://tincapp.pacien.org/)
		* Requires editing text files on the phone :(
* iOS (sort of)
  * via [Cydia](https://www.tinc-vpn.org/packages/cydia/)

## Servers
Every client is a server.

## Self-Hosting
Yes. Only self-hosted.

## OSI Layer[s]
* 2 - In some `mode`s it is a layer 2 mesh
	* These modes do not allow direct peer to peer communication when both peers are behind NAT (IIRC - haxwithaxe).
* 3 - In most `mode`s it is a layer 3 mesh
	* Some or all of these modes make it possible to have direct peer to peer communication when both peers are behind NAT (with a third peer directly accessible to both).

## NAT Traversal
Partial - Available in some modes. A mutually accessible peer is required in modes that allow direct peer to peer communication.

## Routing/Firewall
* Does it route directly peer to peer? If so then, when?
	* Yes. Sometimes.
* Does it create a mesh?
	* Yes
* Does it isolate groups of clients/servers?
	* No. Not on it's own.
* Does it filter access to ports based on the origin?
	* No.

## Setup Notes
* Tinc v1.1 (pre18 at time of writing) is really super simple to setup. A tiny bit of RTFM can get a very fancy mesh overlay network with next to no work.
* It does not lend itself to automation with Ansible unless you want to rely on configuring it entirely with config files in which case it ceases to be simple and easy.
* A separate script or external config is needed to get the interface up.
* Multiple Tinc networks can run on a single machine without jumping through hoops.

## Performance
* Not as good as plain wireguard but still pretty good.

### Speed
Not benchmarked here yet.

### Notes
* Very Very stable performance

## Notes
* The project seems to be dead but it's still very nice. As of January 2024 the last commit was in 2021. Haxwithaxe will be sad if that's a permanent situation.

