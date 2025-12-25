[[Cloudflare Tunnel]]

Cloudflared established _outbound connections_ which are tunnels between your resources and Cloudflare's global network.

Tunnels are persistent objects that route traffic to DNS records. Within the same tunnel, you can run as many _cloudflared_ processes (connectors) as needed.

These processes will establish connections to Cloudflare and send traffic to the nearesst Cloudflare data center.