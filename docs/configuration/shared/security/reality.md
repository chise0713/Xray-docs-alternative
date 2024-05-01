# REALITY

### Structure

```json
{
  "dest": "example.com:443",
  "xver": 0,
  "serverNames": ["example.com", "www.example.com"],
  "privateKey": "",
  "serverName": "",
  "publicKey": ""
}
```

### Fields

#### dest

String, destination address and port.

#### xver

Int, one of `0` `1` `2`, send [proxy protocol](https://www.haproxy.org/download/1.8/doc/proxy-protocol.txt).

#### serverNames

==Server Only==

String array, server names.

#### privateKey

==Server Only==

String, the private key.

#### serverName

==Client Only==

String, the server name to send.

#### publicKey

==Client Only==

String, the public key.