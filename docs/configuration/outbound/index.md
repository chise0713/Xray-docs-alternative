# Inbound

### Structure

```json
{
  "outbounds": [
    {
      "sendThrough": "",
      "protocol": "",
      "settings": {},
      "tag": "",
      "streamSettings": {}
    }
  ]
}
```

### Fields

#### sendThrough

Send through address, an IP address at localhost.

#### protocol

| Protocol        | Format                                     |
| --------------- | ------------------------------------------ |
| `vless`         | [VLESS](./protocol/vless/)                 |

#### tag

The tag of the inbound.