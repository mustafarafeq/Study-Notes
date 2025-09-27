# Border Gateway Protocol

What is Border Gateway Protocol or BGP?
- Border gateway protocol is a routing protocol that controls how data flows from point A to points B and C.
- Responsible for choosing the shortest path between networks, in order to direct network traffic from one network to another.

### ASN = Autonomous System Number
- Autonomous System is just another name for a network or collection of networks.

- BGP identifies the different entities within these AS's (that have ASN's)

BGP operates over TCP (Transmission Control Protocol) using port 179. It is not however automatic and peering, aka connection between multiple ANS's, must be configured manually.

- BGP is a path-factor protocol meaning it exchanges the best path to a destination between peers (ASN's) which is called the ASPATH.

Within cloud environments like AWS, BGP is referred to as either:
- iBGP = internal BGP = Routing within an Autonomous System
- eBGP = external BGP = Routing between an Autonomous System

In Summary: BGP is a routine protocol (protocol = set of software rules) that advertises the shortest path between or within AS's. It is what Direct Connect and Dynamic VPNS use in AWS.