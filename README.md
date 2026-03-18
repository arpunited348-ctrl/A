# APR United + SootheAI — Domain-Ready Final Starter

This package gives you two deployable Next.js apps prepared for your production domain structure:

- `apps/apr-united-web` → deploy to **aprunited.io**
- `apps/sootheai-web` → deploy to **sootheai.aprunited.io**

## What is included

- APR United company website
- SootheAI product landing + core app shell
- Supabase SQL schema and RLS policies
- Deployment checklist for Cloudflare + Vercel + Supabase
- `.env.example` files for both apps

## Domain mapping

| Domain | Target |
|---|---|
| `aprunited.io` | APR United Vercel project |
| `www.aprunited.io` | Redirect to `aprunited.io` |
| `sootheai.aprunited.io` | SootheAI Vercel project |

## Quick deploy order

1. Create a Supabase project.
2. Run `supabase/schema.sql` and `supabase/policies.sql`.
3. Create two Vercel projects from the two app folders.
4. Add environment variables from each `.env.example`.
5. Point Cloudflare DNS to Vercel.
6. Replace placeholder branding/contact data.
7. Deploy.

## Important

I cannot log into your Cloudflare, Vercel, Supabase, or domain accounts from inside this chat, so this package is **domain-ready** but not directly connected by me. Once you add your keys and DNS records, it is ready to deploy.

## Local development

From the monorepo root:

```bash
npm install
npm run dev:apr
npm run dev:soothe
```
