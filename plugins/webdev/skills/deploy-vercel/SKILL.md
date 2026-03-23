---
name: deploy-vercel
description: Deploy a project to Vercel with build verification
disable-model-invocation: true
---

# Deploy to Vercel

Deploy a client website to Vercel with pre-deploy checks.

## Steps

### 1. Pre-deploy Checks
- Verify the project builds locally without errors
- Check environment variables are set (not committed to repo)
- Verify `.gitignore` includes sensitive files
- Check that the framework is detected correctly (Next.js, Nuxt, Astro, etc.)

### 2. Deploy
- If project exists on Vercel — deploy to existing project
- If new — create project, link repo, configure build settings
- Use preview deployment first, then promote to production

### 3. Post-deploy Verification
- Check deployment status and build logs
- Verify the site loads (fetch homepage)
- Check for build warnings or errors in logs
- Verify environment variables are applied

## Input

- Project directory or repo URL
- Environment: preview / production (default: preview)
- Environment variables to set (optional)

## Output

```
## Deploy: [project name]

Status: ✅ Success / ❌ Failed
URL: [deployment URL]
Environment: preview / production
Build time: [duration]

Checks:
- [✅/❌] Build completed
- [✅/❌] Site loads
- [✅/❌] No build warnings

[If failed: error details and suggested fix]
```
