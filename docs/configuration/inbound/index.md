# Inbound

### Structure

```json
{
  "inbounds": [
    {
      "listen": "",
      "port": 443,
      "protocol": "",
      "settings": {},
      "streamSettings": {},
      "tag": "",
      "sniffing": {}
    }
  ]
}
```

### Fields

#### listen

==Required==

Listen address, either an IP address or a Unix domain socket.

#### listen_port

==Required==

Listen port.

#### protocol

| Protocol        | Format                                     |
| --------------- | ------------------------------------------ |
| `vless`         | [VLESS](./protocol/vless/)                 |

#### tag

The tag of the inbound.