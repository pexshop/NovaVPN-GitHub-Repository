# Real VPN node deployment checklist

This repository does not yet operate VPN tunnels. A production VPN requires:
1. Linux VPS nodes in the regions you intend to advertise.
2. WireGuard installed and maintained on each node.
3. IPv4/IPv6 forwarding, NAT, firewall and DNS configuration.
4. Client keypairs generated client-side where possible; never store plaintext private keys in the web app.
5. A narrowly scoped provisioning agent to add/revoke public-key peers and allocate tunnel addresses.
6. Strong service authentication, short-lived signed requests or mTLS, rate limits, audit logs and secret rotation.
7. Node health monitoring, capacity controls, abuse response, privacy/retention policy and incident response.
8. Real-device tests on iOS, Android, Windows and macOS, including DNS/IPv6 leak tests, kill switch and key revocation.

Do not label a location available until its node is deployed and monitored. Do not claim "no logs" until the actual infrastructure and retention behavior have been audited.
