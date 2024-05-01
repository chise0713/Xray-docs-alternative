# Rule

### Structure

```json
{
  "domain": [],
  "ip": [],
  "port": "",
  "sourcePort": "",
  "network": "",
  "source": [""],
  "inboundTag": [""],
  "outboundTag": ""
}
```

### Fields

#### domain

String array, each item is a domain match.

[Domain Name Format](/configuration/shared/match.md)

#### ip

String array, each item is a IP match.

[Predefined IP lists](https://xtls.github.io/en/config/routing.html#predefined-domain-lists)

#### port

String, format as `53` `53,54` `53-55`

#### sourcePort

String, format is the same as above.

#### network

One of `tcp` `udp` `tcp,udp`

#### source

String array, each item is a source IP match.

[Predefined IP lists](https://xtls.github.io/en/config/routing.html#predefined-domain-lists)

#### inboundTag

String array, each item is a inbound tag match.

#### outboundTag

==Required==

String, tag of the target outbound.
