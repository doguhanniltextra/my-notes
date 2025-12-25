Cloudflare Tunnel provides you with a secure way to connect your resources to Cloudflare without a publicly routable IP address. With Tunnel, you do not send traffic to an external IP -- instead, a lightweight daemon in your infra (cloudflared) creates _outbound-only connections_ to Cloudflare's global network. 

Cloudflare Tunnel can connect HTTP web servers, SSH servers, remote desktops, and other protocols safely to Cloudflare. This way, your origins can serve traffic through Cloudflare without being vulnerable to attacks that bypass Cloudflare.

Check: [[SSH Reverse Tunneling]] 


