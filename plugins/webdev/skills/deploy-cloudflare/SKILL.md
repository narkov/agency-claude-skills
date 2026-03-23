---
name: deploy-cloudflare
description: Deploy a project to Cloudflare Pages or Workers
disable-model-invocation: true
---

# Deploy to Cloudflare

Deploy a client website to Cloudflare Pages or a Worker to Cloudflare Workers.

## Modes

### Cloudflare Pages (static sites, SSR frameworks)
1. Check project type and build command
2. Create or update Pages project
3. Deploy and verify

### Cloudflare Workers (APIs, edge functions)
1. Verify wrangler.toml config
2. Check bindings (KV, D1, R2 if used)
3. Deploy and verify

## Steps

### 1. Pre-deploy
- Verify build succeeds locally
- Check wrangler.toml or pages config
- Verify environment variables / secrets are set
- Check custom domain configuration

### 2. Deploy
- Use Cloudflare MCP tools to deploy
- For Pages: trigger build from repo
- For Workers: deploy worker code

### 3. Post-deploy
- Verify deployment is live
- Check custom domain SSL status
- Test key endpoints / pages

## Input

- Project directory
- Type: pages / workers (auto-detect if possible)
- Environment: preview / production

## Output

```
## Cloudflare Deploy: [project]

Type: Pages / Workers
Status: ✅ Live
URL: [deployment URL]
Custom domain: [domain] — SSL: ✅ Active

Checks:
- [✅/❌] Build completed
- [✅/❌] Site accessible
- [✅/❌] Custom domain resolves
- [✅/❌] SSL active
```
