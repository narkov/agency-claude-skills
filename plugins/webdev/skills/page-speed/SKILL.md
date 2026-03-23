---
name: page-speed
description: Analyze page speed issues and suggest optimizations
disable-model-invocation: true
---

# Page Speed Analysis

Analyze a website's performance and provide optimization recommendations.

## Steps

1. If the site is accessible, fetch key pages (homepage, main landing pages)
2. Check for common performance issues:
   - Image sizes and formats
   - Number of HTTP requests
   - JavaScript bundle sizes
   - CSS delivery method
   - Font loading strategy
   - Third-party scripts impact
3. If project code is available, review build configuration:
   - Bundler settings (webpack/vite/next.config)
   - Image optimization pipeline
   - Code splitting setup
   - Caching strategy

## Output

```
## Page Speed Analysis: [site]

### Current Issues
| Issue | Impact | Pages Affected | Fix Effort |
|-------|--------|---------------|------------|

### Optimization Plan (by priority)
1. [Quick win — highest impact, low effort]
2. ...

### Expected Improvement
- LCP: [current] → [estimated]
- CLS: [current] → [estimated]
```
