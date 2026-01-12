# mcp-registry Header

This repo deploys a custom MCP Registry based on the reference implementation https://github.com/modelcontextprotocol/registry.

That one deploys into either GCP or as a "local" deployment with Minio, so this repo is a point-in-time conversion of their docker-compose.yml into a Kubernetes manifest, with a fixed seed data file in the [data](./data) directory

The 3rd party reference implementation allows modification of MCP data stored in Postgres via admins, whereas we would like a more restrictive version changed only via Pull Request to this repo.

