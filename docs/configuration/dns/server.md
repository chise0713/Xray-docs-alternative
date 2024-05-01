### Structure

```json
{
  "servers": [
    "8.8.8.8"
    {
      "address": "1.2.3.4",
      "port": 5353,
      "domains": ["domain:xray.com"],
      "expectIPs": ["geoip:cn"],
      "skipFallback": false,
      "clientIP": "1.2.3.4"
    }
  ]
}
```

### Fields

#### address

The address of the dns server.

| Protocol              | Format                      |
| --------------------- | --------------------------- |
| `TCP`                 | `tcp://1.0.0.1`             |
| `UDP`                 | `8.8.8.8`                   |
| `HTTPS`               | `https://1.1.1.1/dns-query` |
| `QUIC`                | `quic://dns.adguard.com`    |

#### port

The port number of the DNS server.
This item is not applicable when using DOH, DOHL, or DOQL modes, and non-standard ports should be specified in the URL.

#### domains

A list of domain names. The domain names in this list will be queried using this server first.

[Domain Name Format](../shared/match.md)
