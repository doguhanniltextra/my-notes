[[Cloudflare Tunnel]]

- Tunnel: A tunnel is a secure, outbound-only pathway you can establish between your origin and Cloudflare's global network. Each tunnel you create will be assigned a _name_ and a _UUID_.
- Tunnel UUID:  A tunnel UUID is an alphanumeric, unique ID assigned to a tunnel. The tunnel UUID can be used whenever you need to reference a specific tunnel.
- Tunnel Name: A tunnel name is a unique, user-friendly identifier that you choose for a tunnel. Since a tunnel can proxy traffic to multiple services, tunnel names do not need to be hostnames. For example, you can assign your tunnel a name that represent your application/network, a particular server, or the cloud env where it runs.
- Connector: The connector, referred to as _cloudflared_, establishes connectivity from your origin server to the Cloudflare global network. The connector offers high availability by creating four long-lived connections to two distinct data center within Cloudflare's global network. This built-in redundancy means that if an individual connection, server, or data center goes down, your origin remains available.
