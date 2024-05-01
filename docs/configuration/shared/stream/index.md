# streamSettings

### Structure

```json
{
  "streamSettings": {
    "network": "tcp",
    "security": "none",
    "tlsSettings": {},
    "tcpSettings": {},
    "wsSettings": {},
    "httpSettings": {},
    "grpcSettings": {},
    "realitySettings": {},
    "httpupgradeSettings": {},
    "sockopt": {}
  }
}
```

### Fields

#### network

One of `tcp` `udp`

Defaults to `tcp`

#### security

One of `tls` `reality` `none`

Defaults to `none`