# Domain Deploy Checklist

## Cloudflare DNS

### APR United
- A record: `@` → `76.76.21.21`
- CNAME: `www` → `cname.vercel-dns-0.com`

### SootheAI
- CNAME: `sootheai` → `cname.vercel-dns-0.com`

## Vercel

### Project 1
- Root directory: `apps/apr-united-web`
- Custom domain: `aprunited.io`
- Add redirect domain: `www.aprunited.io`

### Project 2
- Root directory: `apps/sootheai-web`
- Custom domain: `sootheai.aprunited.io`

## SSL/TLS
- In Cloudflare, use **Full (strict)**

## Env vars
- Add `.env.example` values into each Vercel project

## Final checks
- Homepage loads
- Signup page loads
- Chat page loads
- SSL is valid
- No mixed-content warnings
- Contact email updated
- Privacy + Terms pages customized
