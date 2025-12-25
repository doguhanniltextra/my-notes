[[How Cloudflare Tunnel Works?]]

[[Cloudflare Tunnel]] uses an outbound-only connection model to enable bidirectional communication. When you install and run _cloudflared_, it initiates an outbound connection through your firewall from the origin to the Cloudflare global network.

Once the connection is established, traffic flows in both directions over the tunnel between your origin and Cloudflare. Most firewalls allow outbund traffic by default. _cloudflared_ takes advantage of this standard by connection out to the Cloudflare network from the server you installed cloudflared on.

You can then configure your firewall to allow only these outbound connections and block all inbound traffic, effectively blocking access to your origin from anything other than Cloudflare. This setup ensures that all traffic to your origin is securely routed through the tunnel.