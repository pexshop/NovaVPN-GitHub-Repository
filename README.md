# NovaVPN

Responsive multi-platform VPN service website starter.

## Included
- Responsive landing page for iOS, Android, Windows and macOS
- Cloudflare Worker API starter
- Cloudflare D1 schema for accounts, devices, VPN nodes and sessions
- WireGuard deployment checklist

## Important
This repository is a website/API starter, not an operating VPN. A real encrypted VPN requires deployed WireGuard nodes, routing/NAT, firewall and DNS configuration, secure device-key provisioning, authentication, monitoring and abuse controls. Cloudflare Workers alone do not create a VPN tunnel.

## Deploy the website
Connect this repository to Cloudflare Pages. Set the build output directory to `public`; no build command is needed.

## Deploy the API
See `worker/README.md`. Replace the D1 database ID in `worker/wrangler.toml` before deployment.
