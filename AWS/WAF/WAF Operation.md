
[[AWS]]

Unlike a traditional firewall that operates at Layer 3 or 4, a WAF inspets the content of HTTP requests. It looks inside the headers, cookies, and POST bodies to identify malicious patterns.
- Positive Security Model (Allowlist): Only allows traffic that matches known _good_ patterns.
- Negative Security Model (Blocklist): Blocks traffic that matches known _bad_ signartures.
- Architectural Placement: It sits between the external internet and your web server, acting as a reverse proxy.
