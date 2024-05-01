# Inbound

### Structure

```json
{
  "routing": {
    "domainStrategy": "AsIs",
    "rules": [],
    "balancers": []
  }
}
```

### Fields

#### domainStrategy

One of `AsIs` `IPIfNonMatch` `IPOnDemand`

- `AsIs`: As is.
- `IPIfNonMatch`: Use domain to match first, if it didn't match any of domain rules, it will resovle domain to IP address then match rules again.
- `IPOnDemand`: Resovle domain to IP then match.
