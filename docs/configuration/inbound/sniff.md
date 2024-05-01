# Sniff

### Structure

```json
{
  "sniffing": {
    "enabled": true,
    "destOverride": [],
    "domainsExcluded": [],
    "routeOnly": false
  }
}
```

### Fields

#### enabled

Enable the sniffer.

#### destOverride

One of `http` `tls` `quic`

Type of traffic needs to be sniff.

When `routeOnly` set to `false`, override the connection destination address with the sniffed domain.

#### domainsExcluded

The destination address of these will not be override.

==DOSE NOT== support [shared domain matcher](/configuration/shared/match/)

#### routeOnly

Keep the target address as the IP address.

See [above](#destoverride).

