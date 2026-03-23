---
name: setup-domain
description: Configure domain, DNS records, and SSL for a client website
disable-model-invocation: true
---

# Domain Setup

Configure a custom domain for a client website — DNS, SSL, redirects.

## Input

- Domain name
- Hosting platform: Vercel / Cloudflare / other
- Subdomains needed (www, blog, app, etc.)

## Steps

### 1. Domain Availability (if new)
- Check if domain is available and pricing
- Suggest alternatives if taken

### 2. DNS Configuration
- Determine required DNS records based on platform:
  - **Vercel**: A record → 76.76.21.21, CNAME www → cname.vercel-dns.com
  - **Cloudflare Pages**: CNAME → [project].pages.dev
  - **Custom hosting**: A record → server IP
- List all records to add/change
- Verify propagation

### 3. SSL
- Verify SSL certificate is issued (automatic on Vercel/CF)
- Check for mixed content issues
- Verify HTTPS redirect works

### 4. Redirects
- Configure www → non-www (or vice versa)
- Set up HTTP → HTTPS redirect
- Old domain → new domain redirect (if migration)

## Output

```
## Domain Setup: [domain]

### DNS Records to Configure
| Type | Name | Value | TTL | Status |
|------|------|-------|-----|--------|

### SSL
Status: ✅ Active / ⏳ Pending / ❌ Not configured
Issuer: [Let's Encrypt / Cloudflare / etc.]

### Redirects
- HTTP → HTTPS: ✅
- www → apex: ✅
- Old domain: [status]

### Verification
- [✅/❌] Domain resolves
- [✅/❌] SSL valid
- [✅/❌] No mixed content
```
