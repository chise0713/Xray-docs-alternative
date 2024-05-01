# Log

### Structure

```json
{
    "log": {
        "access": "access.log",
        "error": "error.log",
        "loglevel": "debug",
        "dnsLog": true
    }
}
```

### Fields

#### access / error

Output file path. Will not write log to console after enable.

#### loglevel

Log level. One of: `debug`  `info`  `warning`  `error`  `none`.

#### dnsLog

Enable dns log output.