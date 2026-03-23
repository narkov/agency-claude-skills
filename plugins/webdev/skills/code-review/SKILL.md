---
name: agency-code-review
description: Review website code for quality, performance, and SEO best practices
disable-model-invocation: true
allowed-tools: Read, Grep, Glob, Bash
---

# Agency Code Review

Review client website code focusing on what matters for agency deliverables.

## Focus Areas

### 1. Performance
- Unoptimized images (missing width/height, no lazy loading, not WebP)
- Render-blocking CSS/JS
- Excessive DOM size
- Missing caching headers in config

### 2. SEO
- Missing or hardcoded meta tags
- No semantic HTML (header, nav, main, footer)
- Missing structured data
- JavaScript-rendered content without SSR/SSG

### 3. Accessibility
- Missing alt texts
- Poor contrast (if detectable in CSS)
- Missing form labels
- No skip navigation

### 4. Security
- Inline scripts without CSP
- Mixed content (http resources on https)
- Exposed API keys or credentials
- Missing security headers

### 5. Code Quality
- Console.log left in production code
- Unused CSS/JS
- Missing error handling on API calls

## Output

List findings grouped by severity (Critical / Warning / Info) with file:line references and fix suggestions.
