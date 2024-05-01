# FakeIP

### Structure

```json
{
  "example.com": "127.0.0.1",
  "dns.google": ["8.8.8.8", "8.8.4.4"]
}
```

### Fields

```go
map{domain: address} | map{domain: [address1,address2]}
```
A list of static IP addresses, with values consisting of a series of 
```json
"domain": "address" || "domain": ["address 1","address 2"]
```
The address can be an IP or a domain name. When resolving a domain name, if the domain name matches an item in this list:

- If the address of the item is an IP, the resolution result will be that IP.
- If the address of the item is a domain name, this domain name will be used for IP resolution instead of the original domain name.
- If multiple IPs and domain names are set in the address, only the first domain name will be returned, and the rest of the IPs and domain names will be ignored.

[Domain Name Format](../shared/match.md)
