# NovaVPN Worker API

1. Install Wrangler: `npm install -g wrangler`
2. Authenticate: `wrangler login`
3. Create D1: `wrangler d1 create novavpn-db`
4. Replace `REPLACE_WITH_D1_DATABASE_ID` in `wrangler.toml` with the returned ID.
5. Apply schema: `wrangler d1 execute novavpn-db --file=schema.sql`
6. Deploy from this directory: `wrangler deploy`

The API currently exposes `GET /health` and `GET /api/plans`. Authentication and tunnel provisioning are intentionally disabled until a secure identity provider and real WireGuard node manager are installed.
