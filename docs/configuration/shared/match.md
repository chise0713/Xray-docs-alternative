# Domain Name Match

- Plain string: When this string matches exactly, the rule takes effect.
- Regular expression: Starting with `"regexp:"`, the rest is a regular expression. When this regular expression matches the target domain name, the rule takes effect.
- Subdomain: Starting with `"domain:"`, the rest is a domain name. When this domain name is the target domain name or its subdomain, the rule takes effect.
- Substring: Starting with `"keyword:"`, the rest is a string. When this string matches any part of the target domain name, the rule takes effect.

### Examples
#### Plain string:
```json
{
  "example.com": "127.0.0.1",
  "dns.google": ["8.8.8.8", "8.8.4.4"],
  "cloudflare-proxied-site-1.com": "cloudflare-proxied-site-2.com"
}
```
#### Regular expression
```json
{
  "regexp:^e(-|x)hentai.org$": "2606:4700::",
  "cloudflare-proxied-site-[0-9]+.com": "cloudflare-proxied-site-1.com"
}
```
#### Subdomain
```json
{
  "domain:example.com": "2606:4700::"
}
```
#### Substring
```json
{
  "keyword:example.com": "2606:4700::"
}
```