---
name: post-launch
description: Post-launch verification — analytics, indexing, redirects, performance
disable-model-invocation: true
---

# Post-Launch Checks

Comprehensive verification after a website goes live.

## Input

- Website URL
- Is this a new site or redesign/migration?
- Previous URL (if migration)

## Checks

### 1. Analytics & Tracking
- [ ] GA4 is receiving data (check realtime report)
- [ ] All conversion events firing (form submissions, clicks, purchases)
- [ ] Google Tag Manager loading correctly
- [ ] Facebook Pixel / other pixels active (if applicable)
- [ ] Search Console verified and receiving data

### 2. Indexing & SEO
- [ ] robots.txt allows crawling (not blocking important pages)
- [ ] XML sitemap accessible and submitted to GSC
- [ ] Homepage is indexable (no noindex tag)
- [ ] Request indexing for key pages via GSC
- [ ] Check Google cache for homepage

### 3. Redirects (if migration)
- [ ] All old URLs redirect to new equivalents (301)
- [ ] No redirect chains (max 1 hop)
- [ ] No redirect loops
- [ ] Old sitemap URLs all resolve
- [ ] 404 page works for truly missing pages

### 4. Performance
- [ ] Core Web Vitals passing (LCP < 2.5s, CLS < 0.1)
- [ ] Mobile page speed acceptable
- [ ] Images loading correctly (no broken images)
- [ ] CDN active and serving assets

### 5. Functionality
- [ ] All forms submit correctly
- [ ] Contact info is correct (phone, email, address)
- [ ] Social media links work
- [ ] Internal links not broken
- [ ] Mobile menu works
- [ ] Cookie consent banner appears

### 6. Security
- [ ] SSL active on all pages
- [ ] No mixed content warnings
- [ ] Security headers present (HSTS, X-Frame-Options)

## Output

```
## Post-Launch Report: [domain]
Launched: [date]
Type: New site / Migration from [old domain]

### ✅ Passed ([count])
- [list of passed checks]

### ❌ Failed ([count])
- [issue]: [details and fix recommendation]

### ⏳ Manual Verification Needed ([count])
- [items that need human check]

### Priority Fixes
1. [most critical issue]
2. ...
```
