# Speed Testing

**This is a work in progress and in lieu of standardized hardware**

**Preferably re-run all tests on the same hardware**

Test the speed of a VPN by creating 2 VMs with 4 vcpu and 4GB RAM on the same machine with virtual network adapters on a bridge network and running iperf3 between the two.

Take the best 0-10 speed of 3 or more runs as the speed for the comparison chart. If the best is substantially different than the other two something is probably wrong. Start over while trying to figure out the problem until you get consistent results. If consistent results cannot be obtained note that in the chart. Because the network is entirely virtual, performance should be very, very consistent.

The default speed of virtual networks can be very high. 1Gb/s was chosen to help mask any CPU bottlenecking. If the CPU usage is so high it limits a 1Gb/s connection substantially that's important information.
