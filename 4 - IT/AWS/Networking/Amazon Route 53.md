**Amazon Route 53**  
Problem: people use names like example.com, while machines use IP addresses, and you want control over which endpoint a user reaches. Route 53 is AWS's DNS service. It can also register domains and health-check endpoints. Its routing policies are what make it more than a phone book:

- Simple routing returns one answer.
- Weighted routing splits traffic by percentage, which is useful for canary releases.
- Latency-based routing sends users to the fastest region.
- Failover routing switches to a backup when the primary fails.
- Geolocation and geoproximity routing route users by where they are.
- Multivalue routing returns several healthy IPs.
