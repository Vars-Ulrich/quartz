---
aliases:
  - ARP
---
## Overview 
ARP, or Address Resolution Protocol, is a crucial network protocol used in [[IPv4]] for mapping an Internet Protocol address (IP address) to a physical machine address that is recognized in the local network. In simpler terms, it translates IP addresses into Media Access Control (MAC) addresses, which are unique identifiers assigned to network interfaces for communications at the physical layer of a network.

When a device on a local network wants to communicate with another device, it needs to know the MAC address associated with the destination IP address. If the MAC address is unknown, the device broadcasts an ARP request packet to all devices on the local network segment. The device with the matching IP address sends an ARP reply, which includes its MAC address, back to the requester. This information is then stored in the ARP cache of the requesting device for future reference, reducing the need to repeat the ARP request broadcast for subsequent communications.

ARP is a type of protocol used in the network link layer and operates below the network layer, helping to facilitate the flow of information on a local network.