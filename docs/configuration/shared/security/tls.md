# TLS

### Structure

```json
{
  "serverName": "",
  "rejectUnknownSni": false,
  "allowInsecure": false,
  "alpn": [],
  "minVersion": "",
  "maxVersion": "",
  "certificates": [],
  "pinnedPeerCertificateChainSha256": [""]
}
```

### Fields

#### serverName

Server name string.

#### rejectUnknownSni

Enable reject unknown sni.

#### allowInsecure

Enable allow insecure.

#### alpn

```json
{
  "alpn": ["http/1.1","h2"]
}
```

[ALPN](https://en.wikipedia.org/wiki/Application-Layer_Protocol_Negotiation) string array, can be any string you want.

#### minVersion/maxVersion

Max/Min TLS version.

#### pinnedPeerCertificateChainSha256

Pinned peer certificate chain sha256.

### certificates
```json
{
  "certificates": [
    {
      "certificateFile": "/path/to/certificate.crt",
      "keyFile": "/path/to/key.key",
      "certificate": [],
      "key": []
    }
  ]
}
```
!!!warning ""

      Key is server only

#### certificateFile / keyFile

String, path to file.

#### certificate / key

Certificate / Key line array, in PEM format.
