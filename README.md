# vpn-notes
Notes on various VPNs, VPN management, and overlay networks

# Comparisons
*insert table with speeds and stuff here*
| Name                      | Status  | Type    | Layer  | Overhead[\*](#as-measured) (b/s) | NAT Traversal | Self-hostable |
| ------------------------- | ------- | ------- | ------ | -------------------------------- | ------------- | ------------- | 
| [Wireguard](Wireguard.md) | Active  | VPN     | 3      | tbd                              | no            | yes           |
| [Tinc](Tinc.md)           | Unknown | Overlay | 2 or 3 | tbd                              | yes           | yes |
| [Innernet](Innernet.md)   | Active  | Overlay?| 3?     | tbd								| yes           | yes |
| [Tailscale](Tailscale.md) | Active  | Overlay | 3	     | tbd                              | yes           | yes |
| [ZeroTier](ZeroTier.md)   | Active  | Overlay | 3      | tbd                              | yes           | partial       |
| [Netmaker](Netmaker.md)   | Active  | Manager | 3      | tbd                              | yes           | yes |

# Contributing
Add comparisons to the section above.

Details to a Markdown file in the root of the repository with a name that matches the protocol.

Add test data to ``/data``.

Add test scripts to ``/scripts``.

# Footnotes
<a id="as-measured"></a>
\* As measured by testing against a virtual 1Gb/s as described in [METHODOLOGY.md](METHODOLOGY.md).
