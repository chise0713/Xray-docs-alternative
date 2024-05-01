### Structure

```json
{
  "vnext": [
    {
      "address": "",
      "port": 443,
      "users": [
        {
          "id": "",
          "encryption": "none",
          "flow": ""
        }
      ]
    }
  ]
}
```

### Fields

### address

==Required==

The server address.

#### port

==Required==

The server port.

### users
```json
{
  "id": "",
  "encryption": "",
  "flow": ""
}
```

#### id

==Required==

VLESS user id.

#### encryption

==Always be none.==

#### flow

VLESS Sub-protocol.

Available values:

* `xtls-rprx-vision`