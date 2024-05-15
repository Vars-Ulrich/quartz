---
sticker: vault//Media/icons/aws-icons/Route53.svg
---
## Routing Policies

### Simple 
- Use for a single resource that performs a given function for your domain, for example, a web server that serves content for the example.com website.

### Failover
- Use when you want to configure active-passive failover.

### Geolocation
- Use when you want to route traffic based on the location of your users.

### Geoproximity
- Use when you want to route traffic based on the location of your resources and, optionally, shift traffic from resources in one location to resources in another.

### Latency
- Use when you have resources in multiple AWS Regions and you want to route traffic to the Region that provides the best latency with less round-trip time.

### Multi-value answer
- Use when you want Route 53 to respond to DNS queries with up to eight healthy records selected at random.
### Weighted
- Use to route traffic to multiple resources in proportions that you specify.


## How Amazon Route 53 uses EDNS0 to estimate the location of a user

- To improve the accuracy of geolocation, geoproximity, and latency routing, Amazon Route 53 supports the edns-client-subnet extension of EDNS0. (EDNS0 adds several optional extensions to the DNS protocol.) Route 53 can use edns-client-subnet only when DNS resolvers support it:
- When a browser or other viewer uses a DNS resolver that does not support edns-client-subnet, Route 53 uses the source IP address of the DNS resolver to approximate the location of the user and responds to geolocation queries with the DNS record for the resolver's location.
- When a browser or other viewer uses a DNS resolver that does support edns-client-subnet, the DNS resolver sends Route 53 a truncated version of the user's IP address. Route 53 determines the location of the user based on the truncated IP address rather than the source IP address of the DNS resolver; this typically provides a more accurate estimate of the user's location. Route 53 then responds to geolocation queries with the DNS record for the user's location.
