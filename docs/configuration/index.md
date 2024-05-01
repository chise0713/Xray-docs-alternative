# Introduction

Xray uses JSON for configuration files.

### Structure
!!! warning ""

    This dose not present you full configuration.
    
    For all configuration details, visit [xtls.github.io](https://xtls.github.io)


```json
{
  "log": {},
  "dns": {},
  "inbounds": [],
  "outbounds": [],
  "routing": {}
}
```

### Fields

| Key            | Format                          |
| -------------- | ------------------------------- |
| `log`          | [Log](./log/)                   |
| `dns`          | [DNS](./dns/)                   |
| `inbounds`     | [Inbound](./inbound/)           |
| `outbounds`    | [Outbound](./outbound/)         |
| `routing`      | [Routing](./routing/)           |

### Check

```shell
xray run -test
```